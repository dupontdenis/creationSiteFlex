# Flex en Action

## Comment mettre le dernier paragraphe du div flex-block en bas de son conteneur ?

## 🚀Réponse de Copilot

Pour aligner le dernier paragraphe au bas de son conteneur, vous pouvez utiliser la propriété CSS margin-top: auto;. Cela pousse le paragraphe vers le bas du conteneur. Voici comment vous pouvez modifier votre CSS :

```css
.flex-block {
  /* existing styles */
  display: flex;
  flex-direction: column;
}

.flex-block p:last-child {
  margin-top: auto;
}
```

Dans ce code, `.flex-block p:last-child` sélectionne le dernier paragraphe de chaque bloc. `margin-top: auto;` pousse ce paragraphe vers le bas du bloc.

Cpilot pourrait vous proposer d'autre idée. Et vous ?

## 🚀Autre solution de Copilot ( 👿 )

Une autre solution pour aligner le dernier paragraphe au bas de son conteneur consiste à utiliser un élément factice pour pousser le dernier paragraphe vers le bas. Voici comment vous pouvez modifier votre HTML et CSS :

```html
<div class="flex-block">
  <!-- existing content -->
  <div class="dummy"></div>
  <p><!-- last paragraph --></p>
</div>
```

```css
.flex-block {
  /* existing styles */
  display: flex;
  flex-direction: column;
}

.flex-block .dummy {
  flex-grow: 1;
}
```
