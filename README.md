# 🤝 C2P – Coup de Pouce

**Les petites contributions changent de grandes vies.**  
C2P est une application solidaire de dons entre particuliers, facilitant l'entraide pour des besoins urgents ou essentiels.

---

## 📲 Fonctionnalités principales

### 👋 Onboarding
- Présentation du concept en quelques secondes
- Accès rapide : "Je veux aider" ou "J’ai besoin d’un coup de pouce"

### 💬 Déposer un besoin
- Montant, catégorie, description courte
- Engagement moral : redonner quand je le pourrai

### 🎁 Faire un don
- Liste filtrable de besoins
- Dons rapides (1€, 2€, 5€…)
- Paiements via Stripe, Apple Pay, etc.

### 👤 Profil utilisateur
- Donneur : historique, classement, badges
- Demandeur : statut des demandes, encouragements

### 🏆 Communauté & Gamification
- Classements, citations inspirantes, mur de la générosité

---

## 🛠️ Stack technique

| Côté       | Technologie         | Pourquoi                                  |
|------------|---------------------|-------------------------------------------|
| Mobile     | **Flutter (Dart)**  | Multiplateforme, moderne, rapide          |
| Backend    | Firebase            | Auth, Firestore, Storage, FCM             |
| Paiement   | Stripe / PayPal API | Gestion simple des micro-dons             |
| Auth       | Firebase Auth       | Email, Google, Apple                      |
| Admin Panel| Flutter Web / Retool| Modération des demandes                   |

---

## 🗂️ Structure du projet Flutter

lib/
├── main.dart
├── screens/
│ ├── onboarding_screen.dart
│ ├── donate_screen.dart
│ ├── request_screen.dart
│ ├── profile_screen.dart
│ └── ranking_screen.dart
├── widgets/
│ ├── need_card.dart
│ ├── donation_popup.dart
│ └── custom_button.dart
├── services/
│ ├── auth_service.dart
│ ├── firestore_service.dart
│ └── payment_service.dart
├── models/
│ ├── need.dart
│ ├── user.dart
│ └── donation.dart
└── theme/
└── app_theme.dart


---

## 🔐 Sécurité

- Vérification d’identité possible (justificatifs)
- Limitation à 1 demande par mois ou validation manuelle
- Historique sécurisé des dons et demandes
- CGU obligatoires dès inscription

---

## 🚀 Lancement local

```bash
flutter pub get
flutter run
