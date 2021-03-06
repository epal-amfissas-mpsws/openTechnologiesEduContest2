# openTechologiesEduContest2
Έργο για τον 2ο Πανελλήνιο Διαγωνισμό Ανοικτών Τεχνολογιών στην Εκπαίδευση

Η παρούσα πρόταση αφορά την ανάπτυξη ενός «έξυπνου» συστήματος ποτίσματος γλαστρών στο πλαίσιο της καλλιέργειας διαφορετικών φυτών σε ένα περιβάλλον αστικού κήπου (π.χ. μπαλκόνι σπιτιού).


Τίτλος Έργου
-------------
Έξυπνο ποτιστικό σύστημα γλαστρών (multiple plants smart watering system - MPSWS)


Περιγραφή
----------
 Το σύστημα αυτό θα αναλαμβάνει το πότισμα 3 γλαστρών για την καλλιέργεια 3 φυτών με διαφορετικές ανάγκες σε νερό. Οι γλάστρες θα βρίσκονται τοποθετημένες σε σταθερή βάση, η μία δίπλα από την άλλη. 

  Η καρδιά του συστήματος θα είναι ένας μικροελεγκτής Arduino Uno ο οποίος μέσω κατάλληλων αισθητήρων θα λαμβάνει αποφάσεις για το πότισμα της κάθε γλάστρας και μέσω κατάλληλων ενεργοποιητών θα τις υλοποιεί. 

  Το σύστημα θα συνοδεύεται από εφαρμογή κινητής συσκευής (mobile app) που θα χρησιμεύει τόσο για την παραμετροποίηση του συστήματος από τον αστικό καλλιεργητή/χρήστη, όσο και την ενημέρωση αυτού για την κατάσταση του συστήματος.   Συγκεκριμένα μέσω της συνοδευτικής εφαρμογής ο αστικός καλλιεργητής θα ορίζει για κάθε μία από τις 3 γλάστρες τις διαφορετικές παραμέτρους που περιγράφουν τις ανάγκες ποτίσματος του φυτού που καλλιεργείται σε αυτήν: α) το επίπεδο ελάχιστης υγρασίας (κατώφλι) και β) την ποσότητα νερού για το πότισμα. Επίσης μέσω της ίδια εφαρμογής θα λαμβάνει ενημέρωση για την τρέχουσα τιμή της υγρασίας των φυτών, καθώς και για την στάθμη του νερού στο δοχείο ποτίσματος. Η επικοινωνία της κινητής συσκευής που θα εκτελεί την εφαρμογή με τον μικροελεγκτή θα γίνεται μέσω του πρωτοκόλου bluetooth.

  Κάθε γλάστρα θα διαθέτει αισθητήρα υγρασίας (soil moisture sensor). Ο μικροελεγκτής μέσω των αισθητήρων αυτών θα ελέγχει την υγρασία του κάθε φυτού και αν αυτή έχει πέσει κάτω από το κατώφλι της ελάχιστης απαιτούμενης υγρασίας που έχει τεθεί από τον καλλιεργητή, θα δίνει εντολή για πότισμα.

  Το πότισμα θα πραγματοποιείται μέσω δοχείου νερού (τεπόζιτο ποτίσματος). Το σύστημα θα διαθέτει αντλία νερού που θα ενεργοποιείται από τον μικροελεγκτή. Το δοχείο θα τροφοδοτείται με νερό που συλλέγεται από την βροχή μέσω κατάλληλης κατασκευής (υδροσυλλέκτης) ή σε συνθήκες ανομβρίας θα συμπληρώνεται από τον οικιακό καλλιεργητή/χρήστη.

  Το σύστημα θα διαθέτει μηχανισμό ανίχνευσης ύψους στάθμης νερού στο δοχείο (τεπόζιτο) ποτίσματος. Μέσω του μηχανισμού αυτού, ο αστικός καλλιερητής/χρήστης θα έχει εικόνα της ποσότητας του διαθέσιμου νερού, το σημαντικότερο όμως θα ειδοποιείται με σχετική προειδοποίηση όταν η δεξαμενή αδειάζει. Οι ενημερώσεις αυτές θα λαμβάνονται μέσα από την συνοδευτική εφαρμογή κινητής συσκευής (mobile app). Ο μηχανισμός ελέγχου στάθμης αυτός δεν θα βασίζεται σε έτοιμους αισθητήρες του εμπορίου, αλλά θα κατασκευαστεί custom made αισθητήρας πολύ χαμηλότερου κόστους για τις ανάγκες του συστήματος.

  Το προτεινόμενο σύστημα θα διαθέτει μηχανισμό μετακινούμενου σωλήνα ποτίσματος από τη μία γλάστρα του συστήματος στην άλλη. Συγκεκριμένα, το άκρο του σωλήνα ποτίσματος από το οποίο εξέρχεται το νερό (το άλλο άκρο είναι συνδεδεμένο στην αντλία) θα καταλήγει σε μηχανισμό που θα το κινεί μέσω σταθερής διαδρομής (ράγα) πάνω από τις γλάστρες. Όταν θα λαμβάνεται από τον μικροελεγκτή η απόφαση ποτίσματος μίας από τις 3 γλάστρες, ο μηχανισμός αυτός πριν αρχίσει το πότισμα, θα μετακινεί τον σωλήνα ποτίσματος στην κατάλληλη γλάστρα. Η υλοποίησή του θα γίνει με χρήση κινητήρα (motor) και συνοδευτικών υλικών (ιμάντας, ράουλο, μεταλλική βέργα-ράγα).


Λίστα προτεινόμενου εξοπλισμού
-------------------------------
- 1 μικρoελεγκτής Arduino Uno - εκτιμώμενο κόστος  20€ (γνήσιος)
- 1 bluetooth module HC-05 - εκτιμώμενο κόστος 7,5€
- 3 αισθητήρες υγρασίας (soil moisture sensor) - εκτιμώμενο κόστος 3 x 2,5 = 7,5€
- 1 αντλία νερού - εκτιμώμενο κόστος 15€
- 1 κινητήρας (motor) - εκτιμώμενο κόστος 5€
- διάφορα συνοδευτικά υλικά - εκτιμώμενο κόστος 10€ 
    - 1 βάση γλαστρών (πιατάκι ζαρντινιέρας)
    - 3 γλάστρες
    - 1 σωληνας ποτίσματος
    - καλώδια
    - αντιστάσεις
    - τρανζίστορς για μηχανισμό ανίχνευσης στάθμης νερού 
    - ιμάντας, ράουλο, μεταλλική βέργα-ράγα για μηχανισμό μετακινούμενου σωλήνα ποτίσματος


Ενδεικτικό κόστος
----------------
65€


Σχόλια
-------
Η συγκεκριμένη πρόταση συμμετοχής στον διαγωνισμό αποτελεί την αφετηρία μίας προσπάθειας για την δημιουργία μίας ενεργούς ομάδας STEM και Ρομποτικής στο σχολείο μας. Το προτεινόμενο σύστημα πραγματεύεται το ζήτημα της διαχείρισης του φυσικού πόρου του νερού με αειφορικό τρόπο στην περίπτωση της καλλιέργειας διαφορετικών φυτών σε ένα περιβάλλον αστικού κήπου. Ως εκ τούτου εντάσσεται στις θεματικές ενότητες α) της εξοικονόμησης ενέργειας - νερού και β) της αστικής κηπουρικής.

  Μέσα από την ανάπτυξη του προτεινόμενου συστήματος θα επιδιωχθεί η επίτευξη των ακόλουθων παιδαγωγικών στόχων για τους μαθητές και τις μαθήτριες:
1) Η βιωματική προσέγγιση της ανάπτυξης μίας τεχνολογικής λύσης σε ένα περιβαλλοντικό πρόβλημα (αειφορική διαχείριση νερού).
2) Η σύνδεση θεωρητικών γνώσεων με την πραγματικότητα–πρακτική εφαρμογή (αυθεντική μάθηση). 
3) Η καλλιέργεια της κριτικής σκέψης και της δημιουργικότητάς τους.
4) Η ανάπτυξη δεξιοτήτων διερεύνησης και επίλυσης προβλημάτων.
5) Η ανάπτυξη δεξιοτήτων στον προγραμματισμό και την πραγματοποίηση κατασκευών.
6) Η υποστήριξη της ομαδοσυνεργατικότητας.
7) Η ενίσχυση της εξωστρέφειάς τους μέσα από την προβολή της εργασίας τους σε μία κλίμακα ευρύτερη και πέρα από τα όρια του σχολείου (διαγωνιστική κοινότητα).
