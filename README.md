# project
### Το παρόν readme file έχει δημιουργηθεί για την παρουσίαση των αποτελεσμάτων της εργασίας του μαθήματος "Τηλεπισκόπηση & Ανάλυση Εικόνων!!!

Ο δείκτης NDVI μας δείχνει της παραλλακτικότητα που υπάρχει στη καλλιέργεια όσον αφορά τη βλάστηση και παίρνει τιμές από -1 έως 1. Τιμές μικρότερες του 0.1 χαρακτηρίζουν το γυμνό έδαφος, τιμές από 0.2 έως 0.5 υποδεικνύουν την ύπαρξη βλάστησης ενώ πάνω από 0.6, έχουμε πυκνή βλάστηση. Αντίστοιχα, ο δείκτης NDWI, μας επιτρέπει να εντοπίζουμε περιοχές ή σημεία στα οποία υπάρχει νερό. Οι τιμές που λαμβάνει είναι από -1 έως 1. Από -1 έως – 0.3, έχουμε ξηρές επιφάνειες, δίχως ύπαρξη νερού, από -0.3 έως 0, λιγότερο ξηρές επιφάνειες, πάλι χωρίς την ύπαρξη νερού, από 0 έως 0.2 υφίσταται μια μικρή ποσότητα νερού ενώ πάνω από 0.2 έχουμε επιφάνειες με νερό. 

![ClimateEngine](https://github.com/tsemplekas/project/assets/139547500/2f2d9f52-c4af-4460-a556-1eb500c9f745)

Σύμφωνα με το παραπάνω διάγραμμα που δημιουργήσαμε μέσω του Climate Engine, παρατηρούμε ότι στο αγροτεμάχιό μας και τα 3 έτη (2021, 2022, 2023) καλλιεργήθηκε κάποια χειμερινή καλλιέργεια. Αυτό το καταλαβαίνουμε απο την περίοδο που αρχίζει και αυξάνει ο δείκτης NDVI αλλά και απο την περίοδο που μειώνεται. Κατά πάσα πιθανότητα πρόκειται για σκληρό σιτάρι διότι εάν ήταν κριθάρι, τότε θα βλέπαμε νωρίτερα τη περίοδο μείωσης του δείκτη. Τέλος, απο το δείκτη καταλαβαίνουμε ότι το καλλιεργητικό έτος 2023 ήταν πιο όψιμο καθώς παρατηρείται η καθυστέρηση στη μείωση του NDVI κατά την ωρίμανση της καλλιέργειας σε σύγκριση με τα 2 προηγούμενα έτη.

#

Για το 2ο ερώτημα, κατασκευάσαμε έναν ιστότοπο (https://tsemplekas.github.io/project/) στον οποίο παρουσιάζονται 4 δείκτες βλάστησης (GBNDVI, GRNDVI, RBNDVI, WDRVI). Μέσω αυτών των δεικτών, μπορούμε να δούμε τη παραλλακτικότητα που εμφανίζει η καλλιέργειά μας στο αγροτεμάχιο κατά το καλλιεργητικό έτος 2023 και πιο συγκεκριμένα στις 13/4. 

![gbndvi_graph](https://github.com/tsemplekas/project/assets/139547500/b4f0430d-ba05-44a4-a3cf-c2a05612f917)

Οι δείκτες GBNDVI, GRNDVI και RBNDVI σύμφωνα με τη βιβλιογραφία παρουσιάζουν μεγαλύτερη συσχέτιση όσον αφορά τον δείκτη LAI (δείκτης μέτρησης χλωροφύλλης). Και αυτό διότι κυρίως οι μπάντες GREEN και BLUE δείχνουν να αποτυπώνουν με  μεγαλύτερη ακρίβεια την ανακλαστικότητα της βλάστησης σε σχέση με τη RED μπάντα. Εάν το σκεφτούμε πιο διεξοδικά, σε ένα υγιές φύλλο, η RED μπάντα απορροφάται περισσότερο απ’ όλες τις άλλες. Ενώ τη μεγαλύτερη ανακλαστικότητα έχει η NIR και η GREEN. Στο δικό μας αγροτεμάχιο, οι δείκτες GBNDVI και GRNDVI είναι σχεδόν πανομοιότυποι. Αυτό σημαίνει ότι η BLUE και RED μπάντα έχουν πανομοιότυπα ποσοστά ανακλαστικότητας. Όμως, ο δείκτης RBNDVI, μεσοσταθμικά είναι λίγο μεγαλύτερος από τους άλλους 2. Αυτό συνεπάγεται ότι οι μπάντες RED και BLUE έχουν μικρότερα ποσοστά ανακλαστικότητας απ’ ότι η GREEN. 

![grndvi_graph](https://github.com/tsemplekas/project/assets/139547500/79e7059f-9e0d-45bd-b8e0-05b300061711)

Ο δείκτης WDRVI, χρησιμοποιείται για να εξαλείψει το πρόβλημα του saturation που δημιουργείται με το δείκτη NDVI. Πρόκειται στην ουσία για το στάδιο εκείνο της καλλιέργειας όπου οι χρωστικές των φύλλων της καλλιέργειας φτάνουν σε ένα κρίσιμο επίπεδο όπου η ανακλαστικότητα της NIR μπάντας αυξάνεται ενώ η RED μπάντα παραμένει στα ίδια ποσοστά ανακλαστικότητας καθώς ακόμη απορροφάται από τα φυτά. Έτσι ο NDVI δεν είναι τόσο ακριβής σε εκείνα τα στάδια ανάπτυξης της καλλιέργειας. Με τη χρήση ενός συντελεστή βαρύτητας στον τύπο υπολογισμού του NDVI, προσπαθούμε να εξαλείψουμε την αύξηση του ποσοστού ανακλαστικότητας της μπάντας NIR και έτσι να έχουμε μια καλύτερη και ακριβέστερη εικόνα σχετικά με τη παραλλακτικότητα και την υγεία της καλλιέργειας.

![rbndvi_graph](https://github.com/tsemplekas/project/assets/139547500/5999609e-cd9f-4de6-8ae3-cecf78756305)

Η καλλιέργεια του αγροτεμαχίου μας, για τη συγκεκριμένη χρονική περίοδο, δε παρουσιάζει παραλλακτικότητα και αυτό γίνεται εύκολα αντιληπτό καθώς οι ελάχιστες και μέγιστες τιμές έχουν πολύ μικρή διαφορά μεταξύ τους.

![wdrvi_graph](https://github.com/tsemplekas/project/assets/139547500/0da7ce0f-f93c-4020-a4c3-4175c156f254)

Τέλος, οι δείκτες GBNDVI, GRNDVI και RBNDVI παρουσιάζουν αρκετά μεγάλη συσχέτιση μεταξύ τους καθώς οι μέσοι όροι τους είναι πολύ κοντά. Ωστόσο, τη μεγαλύτερη συσχέτιση έχουν οι GBNDVI και GRNDVI.
