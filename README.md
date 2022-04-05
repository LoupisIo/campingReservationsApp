# CampingReservations
A simple Node.js Project for a camping site reservations management
Οδηγίες Εγκατάστασης της εφαρμογής:

Εγκατάσταση Βάσης Δεδομένων
1.1.  Για την υλοποίηση της βάσης δεδομένων χρειάζεται η πρόσβαση σε μία εφαρμογή phpmyAdmin. 
Αν δεν έχουμε πρόσβαση σε μία τέτοια μπορούμε εύκολα να την εγκαταστήσουμε στο υπολογιστή μας. 
1.2. Εγκατάσταση XAMPP
Αν δεν διαθέτουμε πρόσβαση σε μία εφαρμογή phpmyAdmin χρειάζεται να εγκαταστήσουμε το XAMPP
 στον υπολογιστή που επιθυμούμε να τρέξουμε την εφαρμογή. Από από τον σύνδεσμο κατεβάζουμε 
 την εκδοση του 8.0.6 του XAMPP που αντιστοιχεί στο OS μας. Αφού ολοκληρωθεί η εγκατάσταση επιτυχώς,
 ανοίγουμε την εφαρμογή και ξεκινάμε τους server MySQL Database και Apache Web server. 
Πηγαίνοντας στην διεθυνηση ‘http://localhost/phpmyadmin/index.php’ και πατώντας
 το Inport μπορούμε να ανεβάσουμε το αρχείο DataBase/paradise_db.sql που δόθηκε μαζί
 με την εργασία ώστε να φορτωθεί η βάση δεδομένων μαζί με τα δεδομένα.
 Στο Character set, επιλέγουμε utf-8.

1.4 Αν δεν έχουμε κάποιο user Account που να είναι γνωστά τα στοιχεία του,
 μπορούμε να δημιουργήσουμε έναν από τον παραπάνω σύνδεσμο. Τα στοιχεία του 
 λογαριασμού που θα δοθούν εδώ είναι τα ίδια που υπάρχουν μέσα στον κώδικα του αρχείου app.js. 
 Αν θέλετε να χρησιμοποιήσετε κάποιον άλλο λογαριασμό θα χρειαστεί να αλλάξετε την δήλωση των 
 στοιχείων συνδεσης στον κώδικα του αρχείου app.js. Γα την δημιουργία του πρότυπου λογαριασμού 
 πηγαίνουμε  User accounts→ Add new User. Και προσθέτουμε τα παρακάτω στοιχεία: 

User name = ‘Web_pro’
Host = ‘localhost’
Password = ‘web_test123’

Και δίνουμε σε αυτό τον χρήστη πλήρη δικαιώματα.

Αφού έχουμε εγκαταστήσει την βάση δεδομένων πρέπει να εγκαταστήσουμε την εφαρμογή. Για μπορέσουμε να το 
κάνουμε αυτό πρέπει να να έχουμε εγκατεστημένο το Node.js 14.17.0 LTS. 
Στην συνέχεια κατευθυνόμαστε από το command line στον φάκελο της εργασίας και τρέχουμε 
τις εξείς εντολές:

npm install package.json

Η παραπάνω εντολή αναλαμβάνει να κατεβάσει όλα τα απαραίτητα για την εφαρμογή modules της Node.js. 
 Αφού ολοκληρωθεί αυτή η διαδικασία τρέχουμε την παρακάτω εντολή για να ξεκινήσει η εφαρμογή:

npm run dev 