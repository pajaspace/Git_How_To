
# Základy práce s Git: Návod

Tento návod obsahuje základní příkazy a pracovní postupy v Gitu

Obsah:<br>
- uvod a pred uvodem jak formatovat a atd
- Jak stahnout z GIT *[Jak stanhout z GITU](https://github.com/pajaspace/Git_How_To/blob/main/Jak_stahnu_z_GITU%20-%20CZ.md)
- nize jsou jednotlive prikazy rozebrane trochu

**Uvod 1**<br>
Spis jeste uplne pred uvodem.<br>
Chtel jsem si na napsat vubec navod ja to funguje atd ...<br>
Nicmene napred je strasne dulezite formatovani textu jako takoveho <br>
Abychom vubec vedeli jak udelat hyperlink a velky text atd ... <br>

**##Moje zkousky Zkousky##<br>**

## Funguje
 ```I love supporting the **[EFF](https://eff.org)**.```<br>
I love supporting the **[EFF](https://eff.org)**.<br> <br> 
```This is the *[Markdown Guide](https://www.markdownguide.org)*```<br>
This is the *[Markdown Guide](https://www.markdownguide.org)*.<br><br> 
```This is the [link](https://www.example.com/my%20great%20page) ```<br>
[link](https://www.example.com/my%20great%20page) <br>

Jeste jednou pro shrnuti v kodu
```bash
I love supporting the **[EFF](https://eff.org)**.<br>
This is the *[Markdown Guide](https://www.markdownguide.org)*.<br>
[link](https://www.example.com/my%20great%20page) <br>
```
**[Celkovy navod zde na linku Markdownguide](https://www.markdownguide.org/cheat-sheet/)**


# Co me nefunguje ... jsou odkazky na jednotlive sekce v dokumentu , priklady nize # <br><br> 

## Nefunguje 
```[Pocatecni Nastaveni](#1. Počáteční nastavení)```<br>
[Pocatecni Nastaveni](#1. Počáteční nastavení)<br><br>
```[Text odkazu](#nazev-sekce)```<br>
[Text odkazu](#nazev-sekce)<br>

```[#1. Počáteční nastavení](##1.).```<br>
[#1. Počáteční nastavení](##1.).<br>

```[##2.Nove repo](##2.).```<br>
[##2.Nove repo](##2.).<br>

```See the section on [`code`](#code).```<br>
See the section on [`code`](#code).<br>




### JAK S GITEM PRIKAZY atd .. ###

##1. Počáteční nastavení

Před použitím Gitu je potřeba nastavit vaše uživatelské jméno a e-mail:

```bash
git config --global user.name "Vaše Jméno"
git config --global user.email "vas.email@example.com"
```

Zkontrolujte aktuální nastavení Gitu:

```bash
git config --list
```

---

## 2. Vytvoření nového repozitáře

### Inicializujte Git repozitář ve složce projektu:
```bash
git init
```

### Přidejte všechny soubory do tzv. staging oblasti:
```bash
git add .
```

### Uložte změny do repozitáře (commit):
```bash
git commit -m "První commit"
```

---

## 3. Práce s existujícím repozitářem

### Klonování existujícího repozitáře:
```bash
git clone https://github.com/uzivatel/jmeno-repozitare.git
```

### Zobrazení aktuálního stavu repozitáře:
```bash
git status
```

### Stažení nejnovějších změn z vzdáleného repozitáře:
```bash
git pull origin main
```

---

## 4. Provádění změn

### Přidání konkrétního souboru do staging oblasti:
```bash
git add nazev_souboru
```

### Přidání všech změněných souborů:
```bash
git add .
```

### Uložení změn do repozitáře (commit):
```bash
git commit -m "Popis změny"
```

---

## 5. Práce s vzdálenými repozitáři

### Přidání vzdáleného repozitáře:
```bash
git remote add origin https://github.com/uzivatel/jmeno-repozitare.git
```

### Odeslání změn do vzdáleného repozitáře:
```bash
git push origin main
```

### Stažení změn z vzdáleného repozitáře:
```bash
git pull origin main
```

---

## 6. Práce s větvemi

### Vytvoření nové větve:
```bash
git branch nazev_vetve
```

### Přepnutí na novou větev:
```bash
git checkout nazev_vetve
```

### Vytvoření a přepnutí na větev v jednom kroku:
```bash
git checkout -b nazev_vetve
```

### Sloučení větve do hlavní větve:
```bash
git checkout main
git merge nazev_vetve
```

---

## 7. Zpětné kroky (Undo Changes)

### Odebrání souboru ze staging oblasti:
```bash
git reset nazev_souboru
```

### Vrácení neuložených změn v souboru:
```bash
git checkout -- nazev_souboru
```

### Resetování posledního commitu (ponechá změny v pracovním adresáři):
```bash
git reset --soft HEAD~1
```

---

## 8. Zobrazení historie

### Zobrazení historie commitů:
```bash
git log
```

### Zobrazení zjednodušené historie commitů:
```bash
git log --oneline
```

---

## 9. Mazání větví

### Smazání lokální větve:
```bash
git branch -d nazev_vetve
```

### Smazání vzdálené větve:
```bash
git push origin --delete nazev_vetve
```

---

## 10. Uživatelské příkazy

### Zobrazení aktuální větve:
```bash
git branch
```

### Zobrazení rozdílů mezi soubory:
```bash
git diff
```

### Zobrazení historie commitů s grafem:
```bash
git log --oneline --graph
```

---

## Další tipy

- Používejte soubor `.gitignore` k ignorování souborů nebo složek, které nechcete zahrnout do repozitáře.
- Commity provádějte často a pište jasné popisy změn.
- Pravidelně stahujte změny z vzdáleného repozitáře, aby byla vaše lokální větev aktuální.

---

Pro pokročilá témata se podívejte na [oficiální dokumentaci Gitu](https://git-scm.com/doc).
```

---

Tento návod pokrývá základy práce s Gitem, od nastavení a prvního commitu až po pokročilejší operace s větvemi a historií. Pokud budete potřebovat další úpravy nebo rozšíření, dejte vědět! 😊
