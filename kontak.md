---
layout: page
title: Formulir Kontak
description: Hubungi redaksi Paciran Lamongan
banner_image: aboutPage.jpg
---


<script type="text/javascript">
var blogId = '209812151361031342';
var contactFormMessageSendingMsg ='Mengirim...';
var contactFormMessageSentMsg = 'Pesan sudah dikirim. Semoga Anda bahagia.';
var contactFormMessageNotSentMsg = 'Pesan tidak dapat dikirim. Coba lagi nanti.';
var contactFormEmptyMessageMsg = 'Bidang pesan harus diisi.';
var contactFormInvalidEmailMsg = 'Alamat email harus valid.'

var widgetLoaded=false;
function sendEmailMsg() {
if(widgetLoaded== false) {
_WidgetManager._RegisterWidget('_ContactFormView', new _WidgetInfo('ContactForm1', 'sidebar', null, document.getElementById('ContactForm1'), {'contactFormMessageSendingMsg': contactFormMessageSendingMsg , 'contactFormMessageSentMsg': contactFormMessageSentMsg , 'contactFormMessageNotSentMsg': contactFormMessageNotSentMsg , 'contactFormInvalidEmailMsg': contactFormInvalidEmailMsg , 'contactFormEmptyMessageMsg': contactFormEmptyMessageMsg , 'title': 'Contact Form', 'blogId': blogId, 'contactFormNameMsg': 'Name', 'contactFormEmailMsg': 'Email', 'contactFormMessageMsg': 'Message', 'contactFormSendMsg': 'Send', 'submitUrl': 'https://www.blogger.com/contact-form.do'}, 'displayModeFull'));
widgetLoaded=true;
document.getElementById('ContactForm1_contact-form-submit').click();
}
return true;
}
</script>
<div class="Form">
<form name="contact-form">
<p></p>
Nama
<br />
<input class="contact-form-name" style="max-width: 400px; width: 100%;" id="ContactForm1_contact-form-name" name="name" size="30" type="text" value="" ></input>

Email
<span style="font-weight: bolder;">*</span><br />
<input class="contact-form-email"style="max-width: 400px; width: 100%;" id="ContactForm1_contact-form-email" name="email" size="30" type="text" value="" ></input>

Pesan
<span style='font-weight: bolder;'>*</span>
<br />
<textarea class="contact-form-email-message" style="max-width: 400px; width: 100%;" id="ContactForm1_contact-form-email-message" name="email-message" rows="5"></textarea>

<input class="contact-form-button contact-form-button-submit" id="ContactForm1_contact-form-submit" onclick="sendEmailMsg()" type="button" value="Kirim" ></input>

<div style="max-width: 400px; text-align: center; width: 100%;">
<p class="contact-form-error-message" id="ContactForm1_contact-form-error-message"></p>
<p class="contact-form-success-message" id="ContactForm1_contact-form-success-message"></p>
</div>
</form>
</div>
