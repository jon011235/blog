---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Willkommen!
**(English translation below)**
Willkommen auf meinem Blog! Ich möchte etwas Neues wagen und meine Gedanken ins Internet "schreien" - in der Hoffnung, mit anderen Menschen in Kontakt zu treten, Diskussionen anzuregen und konstruktive Kritik zu erfahren.

Ich würde mich sehr freuen, wenn du einen meiner Artikel liest und mir eine E-Mail schreibst, besonders wenn du sonst eher zurückhaltend mit Online-Kommentaren bist. Ich bitte dich dann nur darum, dass wir so kommunizieren, wie wir es in einem persönlichen Gespräch von Angesicht zu Angesicht tun würden. 

Mein Eindruck ist, dass die Textform und viele Onlineformate im speziellem es oft zu einfach machen, verletzend und provokativ zu sein - auf eine Art und Weise, die man in einem direkten Gespräch niemals wählen würde. 

Dieser Blog ist - fürchte ich - ein wilder Mix aus Deutsch und Englisch. Sollte dir etwas unklar sein, nutze gerne ein Übersetzungstool oder schreib mir einfach eine Nachricht.


**(German original above)**
Hi, welcome to my blog! While this blog will primarily be in German (I still have a better feeling for nuances in my native language), I warmly invite you to read my articles. If something isn't clear, feel free to use a translation tool.

With this blog I want to try something new and publish some thoughts of mine on the internet. Hoping to engange with new people, inspire some new thoughts and to get critisized in a constructive way. I'm particularly interested in hearing from those who, like me (until now), don't typically comment online. My only request for when you write me, is that you imagine we talk face-to-face when you write me, as I oftentimes have the feeling that writing in general and the internet in particular harm empathy and encourage to easily be more nasty than one would ever be in a face-to-face discussion.




## Empfehlungen
Some books and other media that I recommend (look at the [influential](/influential/) page to learn why). 

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
      <img src="{{ item.img }}" alt="Image">
    {% endif %}
  {% endfor %}
</div>

More at [influential](/influential)

