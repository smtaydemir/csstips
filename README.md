# CSS Tips

Merhaba, kullandığım ve tecrübe edindiğim css ipuçlarını derliyorum. Çok ekstrem bilgiler olmamakla birlikte el altında olması hoş olur diye düşündüm.

## Shorthand

Gereksiz tanımlamalar yapmaktan kurtarır ve tek satırda işlerimizi halletmemizi sağlar. CSS kodumuzu daha düzenli ve temiz bir hale getirir.

###### Font Özellikleri



```css
p{
  font-style: italic;
  font-weight: bold;
  font-size: 16px;
  line-height: 1.5;
  font-family: Arial, sans-serif;
}
```

Kısa Hali;

```css
p{
  font: italic bold 16px/1.5 Arial, sans-serif;
}
```

Shorthand ile ilgili daha fazla örnek için [şuraya](https://developer.mozilla.org/en-US/docs/Web/CSS/Shorthand_properties) bakabilirsiniz.

## Selection Color (Seçim Rengi)

Tarayıcıda imlecimizle bir alanı seçtiğimizde mavi bir renk tonuyla seçim işlemini gerçekleştiriyor. Bunu ``::selection`` ile değiştirebiliyoruz.

```css
::selection{
  background-color:#f00;
  color:#fff;
}

/* Mozilla */
::-moz-selection{
  background-color:#f00;
  color:#fff;
}
```

##Placeholder Text

Bildiğiniz gibi form elemanlarında kullanıcı bir şey girmediğinde şeffaf olarak görünen text'i placeholder ile belirliyoruz. Ancak gelen tasarımda placeholder text'i default olandan farklı bir şekilde biçimlendirilmiş olabiliyor. CSS ile bu text özelliklerini değiştirebiliyoruz.

```css

/** webkit **/
::-webkit-input-placeholder{
  color:#f00;
  background-color:#f5f5f5;
}

/** mozilla **/
::-moz-placeholder{
  color:#f00;
  background-color:#f5f5f5;
}

/** ms **/
::-ms-input-placeholder{
  color:#f00;
  background-color:#f5f5f5;
}
```
