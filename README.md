# NLP Project

Η παρούσα εργασία υλοποιεί μία μελέτη πάνω στην ανακατασκευή νοήματος φυσικής γλώσσας, με στόχο την αξιολόγηση αυτόματων pipelines παραφραστικής και γλωσσικής επεξεργασίας. Μέσα από σύγκριση original, reference και ανακατασκευασμένων εκδοχών, εφαρμόστηκαν λεξιλογικές και σημασιολογικές μετρικές όπως:

- **Jaccard Similarity**
- **Cosine Similarity με BERT embeddings**
- **Οπτικοποίηση t-SNE**

Η όλη προσέγγιση βασίστηκε σε εργαλεία επεξεργασίας φυσικής γλώσσας (NLP) και ενσωματώσεις BERT.

---
## Τεχνολογίες και Εργαλεία

- Python 3.10+
- Poetry
- spaCy – Tokenization, Lemmatization
- HuggingFace Transformers – Text2Text models (T5, Pegasus)
- Scikit-learn – Jaccard & Cosine Similarity, t-SNE
- Matplotlib – 3D Visualization

## Ανοιγμα του project

1. Clone the repository or open the folder in VS Code.
2. Install dependencies using Poetry:
   ```bash
   poetry install
   poetry shell

3. Run the project
Τα notebooks του έργου είναι σχεδιασμένα ώστε να εκτελούνται ανεξάρτητα μεταξύ τους, χωρίς να απαιτείται συγκεκριμένη σειρά εκτέλεσης. Κάθε αρχείο (humarin_pipeline.ipynb, pegasus_pipeline.ipynb, vamsi_pipeline.ipynb, paradoteo_1c_2.ipynb) περιλαμβάνει όλη τη λειτουργικότητα που χρειάζεται για να τρέξει αυτόνομα.

Συγκεκριμένα:

    Τα pipelines humarin, pegasus και vamsi πραγματοποιούν τοπικά τη φόρτωση των μοντέλων και την παραγωγή αναδιατυπώσεων.

    Όλα τα παραγόμενα κείμενα έχουν συγκεντρωθεί και αποθηκευτεί στο notebook paradoteo_1c_2.ipynb για την αξιολόγηση.

    Συνεπώς, το paradoteo_1c_2.ipynb μπορεί να εκτελεστεί απευθείας, χωρίς να προηγηθεί η εκτέλεση των υπόλοιπων notebooks, καθώς βασίζεται στα ήδη αποθηκευμένα δεδομένα.

## Δομή Αρχείων

NLP_Project/
├── alltexts.json                   # original, reference, and generated versions
├── humarin_pipeline.ipynb          # Text reconstruction using Humarin
├── pegasus_pipeline.ipynb          # Text reconstruction using Pegasus
├── vamsi_pipeline.ipynb            # Text reconstruction using Vamsi
├── sentences_reconstruction.ipynb  # ours text reconstruction
├── paradoteo_1c_2.ipynb            # Evaluation & visualizations
├── pyproject.toml                  # Poetry dependency file
├── poetry.lock                     # Poetry lock file
└── README.md                       # this file

## Ομάδα Υλοιποίησης

    Χαράλαμπος Σώρρας – ΑΜ: Π22168

    Παναγιώτα Καραμάνη – ΑΜ: Π22058


