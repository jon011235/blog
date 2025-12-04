---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Willkommen!
**(English translation below)**
Willkommen auf meinem Blog, ich dachte ich probiere mal etwas anderes und fange auch mal an meine Meinung ins Internet zu schreien - in der Hoffnung mit anderen Menschen in Kontakt zu kommen, anzuregen und kritisiert zu werden. Ich würde mich sehr freuen, wenn du einen meiner Artikel liest und mir dann eine Mail schreibst, insbesondere wenn du (wie ich normalerweise) sonst nie im Internet kommentierst. Ich bitte dich nur darum, so wie ich es auch in meinem Artikeln versuche, so zu schreiben, als würdest du "face-to-face" direkt mit einem Menschen reden. Mein Eindruck ist oft, das ein Text oder die diversen anderen online Format es deutlich einfacher machen, verletzend und provokativ zu sein, in einer Art und weise wie man es nicht wäre, wenn man sich gegenüber sitzt. Dieser Blog ist - fürchte ich - ein wilder Mischmasch aus Englisch und Deutsch, sollte etwas für dich nicht verständlich sein nutze einfach ein Übersetzungstool oder schreib mir einfach.

**(German original above)**
Hi, well come to my blog, while it is mostly in German (I still have a better feeling for nuances in German) I invite you to read the articles just as well and use a translation tool.
TODO


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

