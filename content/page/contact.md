---
title: "お問い合わせ"
_build: { list: false }
tags: []
author: toshikun
---
# お問い合わせ
***
ご連絡の際はこちらのフォームからご連絡ください。

**※諸事情によりご連絡が遅れてしまう場合がございますのでその際は各種SNS等からダイレクトメッセージをご利用ください。**
***
<form name="contact" method="POST" action="/page/success" data-netlify="true">
  <p>
    <label>お名前(必須)<br>
    <input type="text" name="name" style="width:100%" required/></label>
  <p>
    <label>メールアドレス(必須)<br>
    <input type="email" name="email" style="width:100%" required/></label>
  </p>
  <p>
    <label>題名<br>
    <input type="text" name="title" style="width:100%" /></label>   
  </p>
  <p>
    <label>お問い合わせ内容<br>
    <textarea name="message" cols="52" style="width:100%" /></textarea></label>
  </p>
  <p>
    <button type="submit">送信</button>
  </p>
</form>
