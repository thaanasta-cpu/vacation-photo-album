# Οι Διακοπές Μας

Private family travel app με Google login, διαχείριση ταξιδιών από κινητό και πρόσβαση ανά ταξίδι.

## Πώς λειτουργεί

- Ο επισκέπτης συνδέεται με τον Google λογαριασμό του.
- Η πρώτη σύνδεση δημιουργεί αίτημα πρόσβασης.
- Ο admin, tha.anasta@gmail.com, εγκρίνει τον χρήστη και επιλέγει τα ταξίδια που θα βλέπει.
- Μόνο ο admin μπορεί να προσθέτει, να αλλάζει ή να διαγράφει ταξίδια και links.

## Μία φορά στο Firebase

1. Στο Authentication > Sign-in method, ενεργοποιήστε το Google.
2. Στο Firestore Database > Rules, αντικαταστήστε όλους τους κανόνες με το περιεχόμενο του αρχείου firestore.rules και πατήστε Publish.
3. Αφού δημοσιευτεί η σελίδα στο GitHub Pages, ανοίξτε Authentication > Settings > Authorized domains και προσθέστε το domain της σελίδας, π.χ. thanast.github.io.

## Δημοσίευση

Ανεβάστε τα αρχεία αυτού του φακέλου σε GitHub repository. Στο repository ανοίξτε Settings > Pages, επιλέξτε Deploy from a branch, branch main και φάκελο /(root).

Η εφαρμογή χρησιμοποιεί Firebase μέσω του configuration στο index.html. Αυτό το configuration είναι αναγνωριστικό του web app, όχι μυστικός κωδικός. Η πραγματική προστασία γίνεται από τους Firestore Security Rules.
