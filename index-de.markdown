---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
lang: de
---

## Willkommen!
Willkommen auf meinem Blog! Ich möchte etwas Neues wagen und meine Gedanken ins Internet "schreien" - in der Hoffnung, mit anderen Menschen in Kontakt zu treten, Diskussionen anzuregen und konstruktive Kritik zu erfahren.

Ich würde mich sehr freuen, wenn du einen meiner Artikel liest und mir eine E-Mail schreibst, besonders wenn du sonst eher zurückhaltend mit Online-Kommentaren bist. Ich bitte dich dann nur darum, dass wir so kommunizieren, wie wir es in einem persönlichen Gespräch von Angesicht zu Angesicht tun würden. 

Mein Eindruck ist, dass die Textform und viele Onlineformate im speziellem es oft zu einfach machen, verletzend und provokativ zu sein - auf eine Art und Weise, die man in einem direkten Gespräch niemals wählen würde. 

Dieser Blog ist - fürchte ich - ein wilder Mix aus Deutsch und Englisch. Sollte dir etwas unklar sein, nutze gerne ein Übersetzungstool oder schreib mir einfach eine Nachricht.


## Empfehlungen
Einige Bücher und Werke, die mich sehr beeindruckt haben (unter [Empfehlungen](/influential/) ist eine ausführliche Liste). 

<style>
.influential-preview {
  display: flex;
  gap: 15px;
  margin: 20px 0;
}

.influential-preview img {
  width: 120px;   /* adjust size */
  height: auto;
  border-radius: 6px;
  object-fit: cover;
}
</style>

<div class="influential-preview">
  {% for item in site.data.influential limit:5 %}
    {% if item.book %}
      <a href="https://openlibrary.org/isbn/{{ item.img }}">
        <img src="https://covers.openlibrary.org/b/isbn/{{ item.img }}-M.jpg"
             alt="Book Cover">
      </a>
    {% else %}
      <a href="{{item.link}}"><img src="{{ item.img }}" alt="Image"></a>
    {% endif %}
  {% endfor %}
</div>

Mehr unter [Empfehlungen](/influential)

