### 🎯 Tema
Dezvoltarea unei platforme inteligente de micro-learning și evaluare asistată de AI pe bază de flashcards.

### 📝 Descriere scurtă
Aplicația permite utilizatorilor să încarce suporturi de curs, din care sistemul generează automat pachete de cărți de studiu (flashcards). În timpul sesiunilor de învățare, studenții introduc răspunsurile sub formă de text liber, iar aplicația le evaluează instantaneu acuratețea, salvând progresul și statisticile de studiu.

### ✅ Cerințe și specificații
* 🔐 Sistem de autentificare și gestiune a conturilor pentru utilizatori
* 📄 Încărcarea și procesarea documentelor de studiu (format text sau PDF)
* ✏️ Adăugare, editare și ștergere manuală a pachetelor de flashcards
* ⚡ Generarea automată de flashcards din documentele încărcate
* 🧠 Desfășurarea de sesiuni de studiu interactive cu introducere de răspunsuri libere
* 📊 Evidența progresului, a istoricului de învățare și a scorurilor obținute
* 🖥️ Interfață grafică responsivă pentru utilizatori
* 🗄️ Stocarea datelor (utilizatori, documente, flashcards, statistici) într-o bază de date relațională

### 💻 Limbajul de programare ales
**Python (FastAPI)** + **React** + **SQLite**

---

### 🤖 Agenți AI

**1. 🪄 Agent generator de conținut educațional (via API)**
* Analizează textul brut extras din documentele încărcate de utilizatori
* Identifică automat conceptele esențiale și formulează întrebări relevante
* Generează pachete structurate de flashcards (perechi întrebare-răspuns)
* Utilizează apeluri API către un model de limbaj de mari dimensiuni (LLM)

**2. 🔬 Agent evaluator de răspunsuri (Model Local)**
* Procesează răspunsurile formulate liber de utilizatori în timpul sesiunilor de studiu
* Calculează similaritatea semantică între răspunsul introdus de student și răspunsul corect
* Oferă feedback instantaneu și obiectiv sub forma unui procentaj de acuratețe
* Rulează exclusiv pe baza unui model NLP local de mici dimensiuni (ex: `sentence-transformers`)
