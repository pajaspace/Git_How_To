Stáhnutí projektu z GitHubu do vašeho počítače je j provádí se příkazem **`git clone`**. 

---

### **1. Najděte URL repozitáře na GitHubu**
1. Otevřete stránku repozitáře na GitHubu.
2. Klikněte na tlačítko **Code** (zelené tlačítko).
3. Vyberte možnost **HTTPS** (nebo SSH, pokud máte SSH klíče nastavené) a zkopírujte URL repozitáře. Například:
   ```
   https://github.com/uzivatel/jmeno-repozitare.git
   ```

---

### **2. Otevřete terminál nebo příkazovou řádku**
- **Windows:** Použijte `Command Prompt` nebo `Git Bash`.
- **Linux/Mac:** Použijte terminál.

---

### **3. Přesuňte se do složky, kam chcete projekt stáhnout**
Použijte příkaz `cd` (change directory) k přesunutí do složky, kam chcete projekt stáhnout. Například:

```bash
cd cesta/k/mistni_slozce
```

---

### **4. Spusťte příkaz `git clone`**
Vložte zkopírovanou URL a spusťte příkaz:

```bash
git clone https://github.com/uzivatel/jmeno-repozitare.git
```

Git stáhne obsah repozitáře do nové složky s názvem projektu.

---

### **5. Přesuňte se do složky projektu**
Jakmile je stahování dokončeno, přejděte do složky projektu:

```bash
cd jmeno-repozitare
```

---

### **6. Zkontrolujte, že Git repozitář funguje**
Zkontrolujte aktuální stav a informace o větvi:

```bash
git status
```

---

### **Shrnutí příkazů**
Pokud chcete rychle stáhnout projekt z GitHubu:
```bash
# Najděte složku, kam chcete projekt stáhnout
cd cesta/k/mistni_slozce

# Stáhněte projekt
git clone https://github.com/uzivatel/jmeno-repozitare.git

# Přesuňte se do složky projektu
cd jmeno-repozitare
```

---

### **Co dělat dál?**
Po stažení můžete:
1. **Prohlédnout si kód:**
   - Pomocí textového editoru (např. VS Code nebo PyCharm).
2. **Upravovat soubory:**
   - Proveďte změny a commitujte je.
3. **Pushnout změny zpět na GitHub:**
   - Pokud máte přístup pro zápis k repozitáři, můžete změny nahrát zpět:
     ```bash
     git add .
     git commit -m "Popis změny"
     git push origin main
     ```

