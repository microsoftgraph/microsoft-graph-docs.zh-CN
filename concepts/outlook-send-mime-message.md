---
title: 使用 Outlook 邮件 API 发送包含 MIME 内容的电子邮件
description: 电子邮件客户端可以通过 Exchange 发送采用 MIME 邮件格式的邮件，并跨多个电子邮件平台进行通信。
author: isvargasmsft
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 7f86ff3ab34c8bdc640fe7874928c2d8400d0e26
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446131"
---
# <a name="send-messages-with-mime-content"></a>使用 MIME 内容发送邮件

许多电子邮件客户端可以通过 Exchange 采用 MIME 邮件格式发送邮件，并跨多个电子邮件平台进行通信。

Outlook 邮件 API 支持对含有 MIME 内容的邮件执行以下操作：
- 发送邮件。
- 发送答复或全部答复邮件。
- 转发邮件。
- 创建草稿邮件。
- 将 S/MIME 签名附加到邮件。
- 使用 S/MIME 加密邮件内容。

> [!IMPORTANT]
> * S/MIME 提供两个关键功能：用于验证发件人和电子邮件内容的数字签名以及防止第三方查看电子邮件内容的邮件加密。
> * 仅以 MIME 邮件格式将 S/MIME 数字签名和加密的内容添加到电子邮件中。

有关 MIME 格式的详细信息，请参阅[获取邮件的 MIME 内容](outlook-get-mime-message.md)。

## <a name="use-cases"></a>用例
| 用例 | API 方法 |
| ------| ----- |
| 创建邮件草稿 | [createMessage](/graph/api/user-post-messages) |
| 发送电子邮件 | [sendMail](/graph/api/user-sendmail) |
| 答复邮件 | [回复](/graph/api/message-reply) |
| 创建草稿以回复邮件 | [createReply](/graph/api/message-createreply) |
| 对邮件执行全部答复 | [全部回复](/graph/api/message-replyall) | 
| 创建草稿以全部回复邮件 | [createReplyAll](/graph/api-reference/api/message-createreplyall) |
| 转发邮件 | [转发](/graph/api/message-forward) |
| 创建草稿以转发邮件 | [createForward](/graph/api-reference/api/message-createforward) | 


## <a name="specify-request-header-and-mime-message-body"></a>指定请求标头和 MIME 邮件正文
可以创建 JSON 或 MIME 格式的[邮件](/graph/api/resources/user)。 在请求标头中指定所需的格式：

- `Content-Type: application/json` 以在请求正文使用 JSON 格式。
- `Content-Type: text/plain` 以在请求正文使用 MIME 格式。

在以 MIME 格式指定正文时，请提供适用的 [Internet 消息标头](https://tools.ietf.org/html/rfc2076) 和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，并在请求正文中以 **base64** 格式对其进行编码。Microsoft Graph 不支持单独编辑或更新 MIME 属性。

## <a name="example"></a>示例
下面是有 Internet 邮件标头（编码前）的 MIME 内容的示例：

<!-- { "blockType": "ignored" } -->

```http
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with with HTTPS; Thu, 6 May 2021
 22:47:18 +0000
Received: from contoso.com (10.194.241.197)
 by contoso.com (10.194.241.197) with
 SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox; Thu, 6 May
 2021 22:47:15 +0000
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Thu, 6 May 2021
 22:47:14 +0000
From: Adele Vance <AdeleV@contoso.com>
To: Alex Wilber <AlexW@contoso.com>
CC: Christie Cline <ChristieC@contoso.com>
Subject: Testing the MIME feature in Graph
Thread-Topic: Testing the MIME feature in Graph
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ==
Date: Thu, 6 May 2021 22:47:14 +0000
Message-ID:
    <4aade2547798441eab5188a7a2436bc1@contoso.com>
Accept-Language: en-US
Content-Language: en-US
X-MS-Exchange-Organization-AuthAs: Internal
X-MS-Exchange-Organization-AuthMechanism: 04
X-MS-Exchange-Organization-AuthSource: contoso.com
X-MS-Has-Attach: yes
X-MS-Exchange-Organization-Network-Message-Id:
    0ffdb402-ec03-42c8-5d32-08d4f37bb517
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
x-ms-publictraffictype: Email
x-originating-ip: [123.456.789.012]
x-ms-traffictypediagnostic: ASDFG12HJ3456:
X-Microsoft-Antispam-Mailbox-Delivery:
    ucf:0;jmr:0;auth:0;dest:I;ENG:(750129)(520011016)(706158)(944506458)(944626604);
X-Microsoft-Antispam-Message-Info:
    D6MmQr/iMMh8YKca2AzC01HqbkKpy3zv5phXo3gGGNXPCyg2KU3OYDhr7eL30FBv0urF1J4B7mf95gtd+vKIdqsYNpvdfV4eJ292mys5pOSmk78/yGSxrHlbOU4gfJ0uGktj1eRoS7rRTDY8J1J2Zch4t/vnfdXgwbrP/lRbTijN1pE93hAPVVMWLyrTk1PczF8McAB/+BkHfFkjEVFjmjeMhZezxyi/Ho5IlfjSrcOasYXgTVkxd6+dUWTXgCueiBIK0tH+FMG+QrIAgSZA7a8F6Os7q1E3yV57sDpbdLDEiyndY9R4ryXRtFjjtqlkDOo0Ss4DGADRYQcs1jmqYrhUwfJuVH97idgW5iVk+MJhpc3Y66MLIkpnjR1jh0XgDOGBLyyocIhhs8PMLpewKxzKzAty85YKUfoqWdr2bLbYWgYdT86F+EWjmbR2mi/tfk6wzQdOCFyDGM2vUVM8EAs+Z34Q5bXAOhlSDgjirgrwgkmUSFR8xvaEws5bbYHzKRiDXw8BD8N9gaLFD8vylIVxCqvmYg9P0+Tol3PzZN/FLOIUNPJrmR67r2qT4QIcGNh2O06dskhCvwWL/imEaqaKbdmBiyjt+jQQ2QvksNSDO8Q97YS5ylTjt2cQyA99
Content-Type: multipart/mixed;
    boundary="_004_MN2PR13MB3152FA5D970E0F158DF41456D5579MN2PR13MB3152namp_"
MIME-Version: 1.0

--_000_MN2PR13MB3152B5FCA9912BEA2E490189D5589MN2PR13MB3152namp_
Content-Type: text/plain; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

Hello Alex,

We are testing the Graph MIME feature.

Kind regards,

Adele

--_000_MN2PR13MB3152B5FCA9912BEA2E490189D5589MN2PR13MB3152namp_
Content-Type: text/html; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

<html>
<head>
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-=
1">
<style type=3D"text/css" style=3D"display:none;"> P {margin-top:0;margin-bo=
ttom:0;} </style>
</head>
<body dir=3D"ltr">
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
Hello Alex,&nbsp;</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
<br>
</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
We are testing the Graph MIME feature.&nbsp;</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
<br>
</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
Kind regards,</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
<br>
</div>
<div style=3D"font-family: Calibri, Arial, Helvetica, sans-serif; font-size=
: 12pt; color: rgb(0, 0, 0);">
Adele</div>
</body>
</html>

--_000_MN2PR13MB3152B5FCA9912BEA2E490189D5589MN2PR13MB3152namp_--

```

以下是相应 base64 编码的字符串：

<!-- { "blockType": "ignored" } -->

```http
UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIHdpdGggSFRUUFM7IFRodSwgNiBNYXkgMjAyMQogMjI6NDc6MTggKzAwMDAKUmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KQogYnkgY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoCiBTTVRQIFNlcnZlciAodmVyc2lvbj1UTFMxXzIsIApjaXBoZXI9VExTX0VDREhFX1JTQV9XSVRIX0FFU18yNTZfQ0JDX1NIQTM4NF9QMjU2KSBpZCAxNS4xLjEzNzQuMCB2aWEgTWFpbGJveDsgVGh1LCA2IE1heQogMjAyMSAyMjo0NzoxNSArMDAwMApSZWNlaXZlZDogZnJvbSBjb250b3NvLmNvbSAKKGZlODA6OjViZjo1MDU5OjRjYTA6NTAxNykgYnkgY29udG9zby5jb20gCihmZTgwOjo1YmY6NTA1OTo0Y2EwOjUwMTclMTIpIHdpdGggbWFwaSBpZCAxNS4wMS4xMzc0LjAwMDsgVGh1LCA2IE1heSAyMDIxCiAyMjo0NzoxNCArMDAwMApGcm9tOiBBZGVsZSBWYW5jZSA8QWRlbGVWQGNvbnRvc28uY29tPgpUbzogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpDQzogQ2hyaXN0aWUgQ2xpbmUgPENocmlzdGllQ0Bjb250b3NvLmNvbT4KU3ViamVjdDogVGhpcyBpcyBhIHRlc3QgaW4gR3JhcGggLSBNSU1FClRocmVhZC1Ub3BpYzogVGhpcyBpcyBhIHRlc3QgaW4gR3JhcGggLSBNSU1FClRocmVhZC1JbmRleDogQVFIVEpXU0hTeXdNelN6OG8wT0p1ZDQ4bkc1MEdRPT0KRGF0ZTogVGh1LCA2IE1heSAyMDIxIDIyOjQ3OjE0ICswMDAwCk1lc3NhZ2UtSUQ6Cgk8NGFhZGUyNTQ3Nzk4NDQxZWFiNTE4OGE3YTI0MzZiYzFAY29udG9zby5jb20+CkFjY2VwdC1MYW5ndWFnZTogZW4tVVMKQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1FeGNoYW5nZS1Pcmdhbml6YXRpb24tQXV0aEFzOiBJbnRlcm5hbApYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1BdXRoTWVjaGFuaXNtOiAwNApYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1BdXRoU291cmNlOiBjb250b3NvLmNvbQpYLU1TLUhhcy1BdHRhY2g6ClgtTVMtRXhjaGFuZ2UtT3JnYW5pemF0aW9uLU5ldHdvcmstTWVzc2FnZS1JZDoKCTBmZmRiNDAyLWVjMDMtNDJjOC01ZDMyLTA4ZDRmMzdiYjUxNwpYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1TQ0w6IC0xClgtTVMtVE5FRi1Db3JyZWxhdG9yOgpYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1SZWNvcmRSZXZpZXdDZm1UeXBlOiAwCngtbXMtcHVibGljdHJhZmZpY3R5cGU6IEVtYWlsCngtb3JpZ2luYXRpbmctaXA6IFsxMjMuNDU2Ljc4OS4wMTJdCngtbXMtdHJhZmZpY3R5cGVkaWFnbm9zdGljOiBBU0RGRzEySEozNDU2OgpYLU1pY3Jvc29mdC1BbnRpc3BhbS1NYWlsYm94LURlbGl2ZXJ5OgoJdWNmOjA7am1yOjA7YXV0aDowO2Rlc3Q6STtFTkc6KDc1MDEyOSkoNTIwMDExMDE2KSg3MDYxNTgpKDk0NDUwNjQ1OCkoOTQ0NjI2NjA0KTsKWC1NaWNyb3NvZnQtQW50aXNwYW0tTWVzc2FnZS1JbmZvOgoJYzRVNno4NjhlZWNha1JUdFBHNzZQemlwTlJJR2w2YWZST1B3TnFHSU1zaW0wWExKaE5vV3BNNks4SzZJNjJvZ0RBalF5cFlPN3BpbmlpVmY5Sm9OWnF1N3pMY3NOUkhrZTBzcWZNYjZzeTRSanhBdzVBekZoQ0duTTJIYmN2cEJQZzhPWi94ZWNxOXd0WXdlNzFYMFJQN3lvdmFIbFlBVUcvMEo4azhmUEdGWWNKa1lHU2xWaXNqQ0ZLMzNBV3BMYm8xb1luRVdlaUtncTU2ZE96QXdSTnVpNzhsNHRQdzBrSW9mYWZnRXBkbnlnekdLYkF1WGkxWXE5T0FCRUNkYzBqRUNjY1VmMUREMFZaVk5sdDE3eHFDUE5UaTYzay9YYkpwUUM2aXdwMHRuSnhJZUhmWjJweG1WdkZGYnJDYWgvamRmTlpTdkN3WkdWNWNqbEFMUWFiYWZacW1mU1VtZW85Nmx4Nks4cHBBOUlVd2hUV3REYkhpTXorU1BxWDBmeUZDbVlSNDlaYktFRnlKanRoODdqU2MwejJPbGNSZC8vV0tySFBJeFZxSEJqbFJEWTJ1M08vOFNreXhOY1ZxcXVsRm5vQ011UjF3ZXFDSzJQYXBkUGJqMllMN0FzWnJNNms0SENnblgvVzZ6NGhGYnlsWkNiUlpUczZBWFJPbSt5VDN1bEdobENja0lLL2ZmNHZFVFRzZksyT3lVREoraGc1NVFWdE81Nit1Y1g1d1hqdDVYazVWZisxQlZTTVNuRzYxVEtKd1hHV21RWnArdTQvc1YrN1k5VzIwZTlWUFNBL1NnWkhOTVVSRXNSbWtBSWs4VURkVHdGTU53SEpHYQpDb250ZW50LVR5cGU6IG11bHRpcGFydC9hbHRlcm5hdGl2ZTsKCWJvdW5kYXJ5PSJfMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfIgpNSU1FLVZlcnNpb246IDEuMAoKLS1fMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfCkNvbnRlbnQtVHlwZTogdGV4dC9wbGFpbjsgY2hhcnNldD0iaXNvLTg4NTktMSIKQ29udGVudC1UcmFuc2Zlci1FbmNvZGluZzogcXVvdGVkLXByaW50YWJsZQoKSGVsbG8gQWxleCwKCldlIGFyZSB0ZXN0aW5nIHRoZSBHcmFwaCBNSU1FIGZlYXR1cmUuCgpLaW5kIHJlZ2FyZHMsCgpBZGVsZQoKLS1fMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfCkNvbnRlbnQtVHlwZTogdGV4dC9odG1sOyBjaGFyc2V0PSJpc28tODg1OS0xIgpDb250ZW50LVRyYW5zZmVyLUVuY29kaW5nOiBxdW90ZWQtcHJpbnRhYmxlCgo8aHRtbD4KPGhlYWQ+CjxtZXRhIGh0dHAtZXF1aXY9M0QiQ29udGVudC1UeXBlIiBjb250ZW50PTNEInRleHQvaHRtbDsgY2hhcnNldD0zRGlzby04ODU5LT0KMSI+CjxzdHlsZSB0eXBlPTNEInRleHQvY3NzIiBzdHlsZT0zRCJkaXNwbGF5Om5vbmU7Ij4gUCB7bWFyZ2luLXRvcDowO21hcmdpbi1ibz0KdHRvbTowO30gPC9zdHlsZT4KPC9oZWFkPgo8Ym9keSBkaXI9M0QibHRyIj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KSGVsbG8gQWxleCwmbmJzcDs8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KPGJyPgo8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KV2UgYXJlIHRlc3RpbmcgdGhlIEdyYXBoIE1JTUUgZmVhdHVyZS4mbmJzcDs8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KPGJyPgo8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KS2luZCByZWdhcmRzLDwvZGl2Pgo8ZGl2IHN0eWxlPTNEImZvbnQtZmFtaWx5OiBDYWxpYnJpLCBBcmlhbCwgSGVsdmV0aWNhLCBzYW5zLXNlcmlmOyBmb250LXNpemU9CjogMTJwdDsgY29sb3I6IHJnYigwLCAwLCAwKTsiPgo8YnI+CjwvZGl2Pgo8ZGl2IHN0eWxlPTNEImZvbnQtZmFtaWx5OiBDYWxpYnJpLCBBcmlhbCwgSGVsdmV0aWNhLCBzYW5zLXNlcmlmOyBmb250LXNpemU9CjogMTJwdDsgY29sb3I6IHJnYigwLCAwLCAwKTsiPgpBZGVsZTwvZGl2Pgo8L2JvZHk+CjwvaHRtbD4KCi0tXzAwMF9NTjJQUjEzTUIzMTUyQjVGQ0E5OTEyQkVBMkU0OTAxODlENTU4OU1OMlBSMTNNQjMxNTJuYW1wXy0t

```

如果要包括文件附件，请将采用 base64 的文件元数据和`Content-Transfer-Encoding`标头附加到 MIME内 容中：

<!-- { "blockType": "ignored" } -->

```http

--_004_MN2PR13MB3152FA5D970E0F158DF41456D5579MN2PR13MB3152namp_
Content-Type: application/vnd.openxmlformats-officedocument.wordprocessingml.document;
    name="Proposed_agenda_topics.docx"
Content-Description: Proposed_agenda_topics.docx
Content-Disposition: attachment; filename="Proposed_agenda_topics.docx";
    size=707560; creation-date="Fri, 07 May 2021 14:06:45 GMT";
    modification-date="Fri, 07 May 2021 14:07:28 GMT"
Content-Transfer-Encoding: base64

UEsDBBQABgAIAAAAIQA9xUZS1AEAALMLAAATAAgCW0NvbnRlbnRfVHlwZXNdLnhtbCCiBAIooAAC
AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA
ZW0yLnhtbC5yZWxzUEsBAi0AFAAGAAgAAAAhAHvzAqPDAAAAKAEAAB4AAAAAAAAAAAAAAAAAVbgK
AGN1c3RvbVhtbC9fcmVscy9pdGVtMy54bWwucmVsc1BLAQItABQABgAIAAAAIQCyOUr/vAYAAIIe
AAATAAAAAAAAAAAAAAAAAFy6CgBjdXN0b21YbWwvaXRlbTIueG1sUEsFBgAAAAAhACEAwwgAAHHB
CgAAAA==

--_004_MN2PR13MB3152FA5D970E0F158DF41456D5579MN2PR13MB3152namp_--

```

## <a name="error-conditions-and-messages"></a>错误条件和邮件

|应用场景|操作|错误代码|错误消息|
|--------|------|----|-------|
| MIME 内容格式错误、丢失 | POST, PUT | 400 | MIME 内容无效的 base64 字符串。 |

## <a name="next-steps"></a>后续步骤

- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- 在 Microsoft Graph v1.0 中 [使用邮件 API](/graph/api/resources/mail-api-overview) 及其 [用例](/graph/api/resources/mail-api-overview#common-use-cases)