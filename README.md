# tbs-backend
backend d'un site web transactionnel dynamique
# Description
API backend sécurisée pour la plateforme e-commerce + réservation, développée avec NestJS, TypeORM, PostgreSQL et JWT Auth.

Ce backend gère :
- Produits & catégories
- Panier & commandes
- Paiements (Orange Money, MTN MoMo, PayPal)
- Module de réservation
- Comptes utilisateurs + rôles (Admin, Client)
- Dashboard admin
- Statistiques
- Notifications (e-mail, SMS)

# Stack Technique-
- NestJS 10
- TypeORM
- PostgreSQL
- JWT + 2FA
- Swagger Documentation
- Nodemailer
- Redis (sessions & cache)

# Structure du projet
```bash
src/
├── auth/
├── users/
├── products/
├── categories/
├── orders/
├── reservations/
├── payments/
├── reviews/
├── uploads/
├── notifications/
├── common/
└── config/
```

# Installation
```bash
git clone <url>
cd backend
npm install
```
# Créer le fichier .env :
```bash
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_USER=postgres
DATABASE_PASS=123456
DATABASE_NAME=ecommerce
JWT_SECRET=supersecret
```

# Scripts utiles
```bash
npm run start:dev   # mode développement
npm run build       # build production
npm run test        # tests unitaires
npm run migration:generate
npm run migration:run
```

# Conventions de commit
```bash
feat: ajout module réservation
fix: corrige bug paiement
chore: MAJ dépendances
refactor: amélioration code service produit
docs: maj readme
```

# Stratégie de branches
Branches recommandées :
```bash
main  → production
dev   → développement
feature/*  → chaque module
```
Exemples :
```bash
feature/auth
feature/products
feature/payments
```
