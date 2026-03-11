# 🎓 Bine ați venit la NeuroDeck

Suntem o echipă de studenți pasionați care construiesc viitorul educației prin micro-learning. **NeuroDeck** este proiectul nostru pentru laboratorul de **Metode de Dezvoltare Software (MDS)**.

Platforma noastră transformă orice suport de curs (PDF/TXT) într-o experiență de studiu interactivă și personalizată, propulsată de **Inteligența Artificială**.

---

## 🚀 Misiunea Noastră

Spre deosebire de aplicațiile clasice de tip flashcards (unde studentul doar apasă un buton "Arată răspunsul"), aplicația noastră îl obligă să *formuleze* răspunsul liber. Sistemul evaluează răspunsul în timp real, oferind un procentaj de acuratețe obiectiv. 

Acest proces este susținut de **doi agenți AI complementari**:

1. 🤖 **Generatorul (LLM API):** Un model generativ avansat care procesează automat documentele încărcate de utilizator și extrage conceptele cheie sub formă de pachete de întrebări și răspunsuri.
2. 🧠 **Evaluatorul (Model NLP Local):** Un model local de procesare a limbajului natural (`sentence-transformers`) care calculează similaritatea semantică (Cosine Similarity) între răspunsul liber tastat de student și răspunsul oficial din curs, oferind o notă instantanee.

---

## 🛠️ Stack-ul Tehnologic

Aplicația urmează o arhitectură modernă de tip Client-Server (REST API), optimizată pentru viteza de răspuns și modularitate.

* **Backend (API):** Python 3, FastAPI, SQLAlchemy
* **Frontend:** React.js + TailwindCSS
* **Bază de date:** PostgreSQL (sau SQLite pentru dezvoltare locală)
* **Integrare AI:** * API-uri externe (OpenAI / Google Gemini) pentru generarea de conținut.
  * Biblioteci locale (`transformers`, `sentence-transformers`) pentru evaluarea semantică.
* **Arhitectură & Procese:** Versionare Git (Git Flow), Teste Automate (`pytest`), Design Patterns (Strategy, Factory, Repository).

---

## 📂 Structura Organizației

Aici veți găsi repository-urile principale ale proiectului nostru:

* 📦 **`NeuroDeck-Backend`**: Codul sursă pentru API-ul REST scris în FastAPI, logica de business, integrarea cu baza de date și implementarea celor doi agenți AI. Conține și suita de teste automate.
* 🖥️ **`NeuroDeck-Frontend`**: Interfața utilizatorului, dezvoltată pentru a fi rapidă, responsivă și intuitivă.
