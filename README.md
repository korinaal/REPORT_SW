
# Data visualization - Τελική Αναφορά

## Αικατερίνη-Γεωργία Αλβάνου Π2015168

* *Link στο αποθετήριο του μαθήματος:* https://github.com/korinaal/sw
* *Link στο αποθετήριο της εφαρμογής:* https://github.com/korinaal/D3js-uk-political-donations
* *Link στη σελίδα με την εφαρμογή:* https://korinaal.github.io/D3js-uk-political-donations/
* *Link στην τελική μου αναφορά:* https://korinaal.github.io/REPORT_SW/

## Σύνοψη


Η παρούσα εργασία έχει ως θέμα την οπτικοποίηση στατιστικών στοιχείων δωρεών σε πολιτικά κόμματα της Μεγάλης Βρετανίας και υλοποιήθηκε στα πλαίσια του μαθήματων Τεχνολογία Λογισμικού. Με τη βοήθεια του github έγινε fork του αποθετηρίου της εργασίας και έπειτα τροποιήθηκε η ιστοσελίδα των δωρεών, σύμφωνα με τα ζητούμενα των εκφωνήσεων. Η ιστοσελίδα αυτή, βασισμένη πάνω στη βιβλιοθήκη D3 της Javascript, καθώς και όλη η διαδικασία της τροποίησής της, αποτελεί ένα σαφές πάραδειγμα συντήρησης και επέκτασης κώδικα. Πάνω στο ήδη υπάρχων αρχείο, προστέθηκαν επιπλέων διαδραστικές δυνατότητες, όπως μεγέθυνση, αυτόματη μετατροπή κειμένου σε ομιλία και ομαδοποιήση ανά μέγεθος δωρεάς, έτσι ώστε το περιεχόμενό του να γίνει πιο προσιτό και κατανοητό από τον χρήστη. 
Αξιοσημείωτο είναι επίσης το γεγονός, ότι μετά την εξοικείωση μου με το Github μέσω της εργασίας, γίνεται αντιληπτό το πόσο δυνατό είναι τελικά το συγκεκριμένο εργαλείο. 

## Διαδικασία Ανάπτυξης

### Παραδοτέο 1 

#### Ζητούμενα στα οποία απαιτούνται αλλαγές στο προσωπικό μου αποθετήριο

* Προστέθηκε ο [σύνδεσμος](https://korinaal.github.io/D3js-uk-political-donations) της εφαρμογής μου στην περιγραφή του αποθετηρίου

* Μετονόμασα το αρχείο full-viz.html σε index.html, ώστε να μην εμφανίζεται η κατάληξη στο url.

* Για την αλλαγή των χρωμάτων στις μπάλες, άλλαξα τον κώδικα στο αρχείο chart.js. Για την αλλαγή των πεδίων άλλαξα τον κώδικα στο style.css. Για λόγους αισθητικής, προσπάθησα να βρω τρία ταιριαστά μεταξύ τους χρώματα και έτσι βοηθήθηκα από το online εργαλείο https://www.sessions.edu/color-calculator/.

![img1](https://user-images.githubusercontent.com/22644422/43684080-26da5cf0-98a2-11e8-8484-5f21830194f6.png)


Ενδεικτική οθόνη:

![colors1](https://user-images.githubusercontent.com/22644422/43974195-7946c3fe-9ce2-11e8-840e-d4a3ed4cbe66.png)

* Προστέθηκε ήχος σε κάθε πάτημα επιλογής ομαδοποίησης. Αρχικά κατέβασα ένα [mp3 αρχείο](https://github.com/korinaal/D3js-uk-political-donations/blob/gh-pages/click.mp3) από την ιστοσελίδα: http://soundbible.com

![im2](https://user-images.githubusercontent.com/22644422/43686172-282df904-98ca-11e8-8c85-be488f7de11d.png)

και έγινε επεξεργασία του αρχείου με τη βοήθεια σχετικού [online εργαλείου](https://audiotrimmer.com/):

![img3](https://user-images.githubusercontent.com/22644422/43686173-2d293cf2-98ca-11e8-9306-55c73f294f60.png)

Στη συνέχεια ο ήχος ανέβηκε στο αποθετήριο και μέσα στον κώδικα του αρχείου html προστέθηκε javascript συνάρτηση που αναπαράγει τον ήχο κατά το πάτημα των κουμπιών.

* Mέσα στο αρχείο chart.js και στο σημείο που αποφασίζονται οι εντολές mouseover και mouseout για τις μπάλες, πρόσθεσα το on "click" και όρισα σχετική συνάρτηση που ανοίγει καρτέλα google αναζήτησης, χρησιμοποιώντας το όνομα του δωρητή. 

* Για να καταφέρω να εφαρμόσω τη μεγέθυνση, επεξεργάστηκα τα αρχεία css και html. Πρόσθεσα κώδικα έτσι ώστε όταν γίνεται hover πάνω από τους παραγράφους να αυξάνεται το μέγεθός τους 30%. Επίσης πρόσθεσα κάποιες βοηθητικές ετικέτες στο αρχείο html για αυτόν το σκοπό. 

![hover](https://user-images.githubusercontent.com/22644422/43972846-6e6fb368-9cde-11e8-8825-cfce08d5af53.png)


* Πραγματοποιήθηκε η αναπαραγωγή της ονομασίας του δωρητή και του ποσού της δωρεάς κατά την μετάβαση του κέρσορα πάνω από τις μπάλες.
Για να επιτευχθεί αυτό, έγινε χρήσης της βιβλιοθήκης ResponsiveVoice.JS και από την [ιστοσελίδα](https://responsivevoice.org/) τους πάρθηκε το κατάλληλο link το οποίο πρόσθεσα στο τέλος του html. Ύστερα τροποποίησα τις συναρτήσεις mouseover και mouseout του chart.js και έβαλα κατάλληλες, της βιβλιοθήκης αυτής, εντολές (συμβουλεύτηκα το API της ιστοσελίδας).

* Προστέθηκε πέμπτο κουμπί στο μενού, για ομαδοποίηση των δεδομένων ανάλογα με το ποσό της δωρεάς στο index.html. Επίσης στο index προστέθηκε νέο div το οποίο περίεχει τους τίτλους για τις ομαδοποίησεις. 
Στο αρχείο chart.js δημιουργήθηκε νέα συνάρτηση, η οποία τοποθετεί τις μπάλες στις κατάλληλες θέσεις ανάλογα με το ποσοστό της δωρεάς. Ακολούθησα τις ήδη υπάρχουσες συναρτήσεις, για βοήθεια πάνω στην κατασκευή της καινούργιας. Τελικά οι δωρεές κατατάσσονται σε τέσσερεις κατηγορίες.
Τέλος, για να εμφανίζονται και οι τίτλοι στις κατάλληλες θέσεις, έγινε η επεξεργασία των θέσεων τους στο αρχείο style.css.

![new-split](https://user-images.githubusercontent.com/22644422/43973583-a5197b7c-9ce0-11e8-84af-5b6b932f01dc.png)



 Ο κώδικας σε όλα τα αρχεία είναι κατάλληλα σχολιασμένος στα σημεία όπου πραγματοποιήθηκαν οι αλλαγές.

#### Ζητούμενα στα οποία απαιτούνται αλλαγές (pull request) στο κοινό αποθετήριο του κώδικα

* Διαγράφηκε το παλιό, και δημηιουργήθηκε εκ νέου το αρχείο [2015168.csv](https://github.com/korinaal/D3js-uk-political-donations/blob/master/participants/2015168.csv) στο φάκελο participants του αποθετηρίου του κώδικα, και έπειτα συμπληρώθηκε με βάση το παράδειγμα.

* Στον φάκελο photos του αποθετηρίου του κώδικα προστέθηκαν 5 φωτογραφίες δωρητών, για τις οποίες δεν έγινε ανάθεση από άλλους συμφοιτητές μου, και τις διαστάσεις των οποίων μετέτρεψα σε 42x42 pixels και την κατάληξη σε .ico.

To [εργαλείο](http://resizeimage.net/) που χρησιμοποιήθηκε για το resize: 

![img4](https://user-images.githubusercontent.com/22644422/43687388-f86358a0-98dc-11e8-979b-b9836b7963c1.png)


Για τα δύο παραπάνω παραδοτέα έκανα pull request από το master branch για να μεταβούν οι αλλαγές μου στο κύριο αποθετήριο της εργασίας.



### Παραδοτέο 2

#### Ζητούμενα στα οποία απαιτούνται αλλαγές στο προσωπικό μου αποθετήριο

* Δημιουργήθηκε νέο div, το οποίο προορίζεται για τις εικόνες των δωρητών μέσα στις οποίες εισέρχεται το ποντίκι, και επιλέχθηκε το position του στο style.css. Έπειτα, στο αρχείο του javascript, έγινε προσθήκη στη συνάρτηση mousover των εντολών που αξιοποιούν το ήδη υπάρχων link της εικόνας του κύκλου και προσθέτουν καινούργιο element εικόνας στο div αυτό. Αποφασίζεται το μέγεθος του κάθε element και προστίθεται η δυνατότητα, μέσω κλικ, να γίνεται ανακατεύθυνση στην google αναζήτηση για τον αντίστοιχο δωρητή. Επίσης με την αποθήκευση του ονόματος του κάθε δωρητή σε λίστα, γίνεται έλεγχος έτσι ώτσε να μην εμφανίζονται διπλτότυπες εικόνες.

Παρακάτω, φαίνεται το τελικό αποτέλεσμα της εφαρμογής της εκφώνησης στην ιστοσελίδα:

![screenshot_1](https://user-images.githubusercontent.com/22644422/45120167-072d7400-b166-11e8-9724-c5a10346a45d.png)

Ο κώδικας σε όλα τα αρχεία είναι κατάλληλα σχολιασμένος στα σημεία όπου πραγματοποιήθηκαν οι αλλαγές.

#### Ζητούμενα στα οποία απαιτούνται αλλαγές (pull request) στο κοινό αποθετήριο του κώδικα

* Έγινε εφαρμογή κίνησης στα στοιχεία μου στο αρχείο index.html του κεντρικού αποθετηρίου του κώδικα το οποίο και επεξεργάστηκε με τη βοήθεια διαφόρων παραδειγμάτων στο internet και έπειτα αφού ελέγχθηκε και δεν υπήρχαν ασυμβατότητες με το κεντρικό, στάλθηκε το pull request.

Η εισαγωγή των στοιχείων στο index φαίνεται παρακάτω:

![kinisi](https://user-images.githubusercontent.com/22644422/44996848-f092eb80-afb2-11e8-90d9-f3aebbfd48a5.png)

* Δημιούργησα επίσης στον φάκελο participants το αρχείο με τον αριθμό μητρώου μου 2015169.html.
Χρησιμοποίώντας το ΑΡΙ του github, έκανα οπτικοποίηση των συνεισφορών που έγιναν από τους χρήστες. Για τον κάθε χρήστη φτιάχτηκε ξεχωριστό τμήμα στην ιστοσελίδα, φαίνεται η φωτογραφία προφίλ του και το σύνολο των συνεισφορών του. Επίσης, κάνοντας κλικ στις φωτογραφίες γίνεται ανακατεύθυνση στα προφίλ των χρηστών. Έγινε pull request στο κεντρικό αποθετήριο.

Η ιστοσελίδα μου φαίνεται παρακάτω:

![paradoteo](https://user-images.githubusercontent.com/22644422/44996990-c988e980-afb3-11e8-83f4-9a1e5bb62dbc.png)

## 

