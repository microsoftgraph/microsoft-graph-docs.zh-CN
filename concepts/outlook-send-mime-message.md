---
title: 发送含有 MIME 内容的电子邮件
description: 电子邮件客户端可以通过 Exchange 以 MIME 邮件格式发送电子邮件。
author: isvargasmsft
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 2e36f84334937a6a3a68f29201c66deae554ecd8
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645885"
---
# <a name="send-messages-with-mime-content"></a><span data-ttu-id="620f9-103">使用 MIME 内容发送邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-103">Send messages with MIME content</span></span>

<span data-ttu-id="620f9-104">许多电子邮件客户端可以通过 Exchange 采用 MIME 邮件格式发送邮件，并跨多个电子邮件平台进行通信。</span><span class="sxs-lookup"><span data-stu-id="620f9-104">Many email clients can send messages through Exchange in a MIME message format and communicate across multiple email platforms.</span></span>

<span data-ttu-id="620f9-105">Outlook 邮件 API 支持对含有 MIME 内容的邮件执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="620f9-105">The Outlook mail API supports the following actions on messages with MIME content:</span></span>
- <span data-ttu-id="620f9-106">发送邮件。</span><span class="sxs-lookup"><span data-stu-id="620f9-106">Send messages.</span></span>
- <span data-ttu-id="620f9-107">发送答复或全部答复邮件。</span><span class="sxs-lookup"><span data-stu-id="620f9-107">Send reply or reply-all messages.</span></span>
- <span data-ttu-id="620f9-108">转发邮件。</span><span class="sxs-lookup"><span data-stu-id="620f9-108">Forward messages.</span></span>
- <span data-ttu-id="620f9-109">创建草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="620f9-109">Create draft messages.</span></span>
- <span data-ttu-id="620f9-110">将 S/MIME 签名附加到邮件。</span><span class="sxs-lookup"><span data-stu-id="620f9-110">Attach S/MIME signatures to a messages.</span></span>
- <span data-ttu-id="620f9-111">使用 S/MIME 加密邮件内容。</span><span class="sxs-lookup"><span data-stu-id="620f9-111">Encrypt message content using S/MIME.</span></span>

> [!IMPORTANT]
> * <span data-ttu-id="620f9-112">S/MIME 提供两个关键功能：用于验证发件人和电子邮件内容的数字签名以及防止第三方查看电子邮件内容的邮件加密。</span><span class="sxs-lookup"><span data-stu-id="620f9-112">S/MIME provides two key features: digital signatures to verify sender and email contents, and message encryption to prevent third parties from viewing email contents.</span></span>
> * <span data-ttu-id="620f9-113">仅以 MIME 邮件格式将 S/MIME 数字签名和加密的内容添加到电子邮件中。</span><span class="sxs-lookup"><span data-stu-id="620f9-113">Add S/MIME digital signatures and encrypted content to emails only in their MIME message format.</span></span>

<span data-ttu-id="620f9-114">有关 MIME 格式的详细信息，请参阅[获取邮件的 MIME 内容](outlook-get-mime-message.md)。</span><span class="sxs-lookup"><span data-stu-id="620f9-114">For more information on MIME format, see [getting MIME content of a message](outlook-get-mime-message.md).</span></span>

## <a name="use-cases"></a><span data-ttu-id="620f9-115">用例</span><span class="sxs-lookup"><span data-stu-id="620f9-115">Use cases</span></span>
| <span data-ttu-id="620f9-116">用例</span><span class="sxs-lookup"><span data-stu-id="620f9-116">Use cases</span></span> | <span data-ttu-id="620f9-117">API 方法</span><span class="sxs-lookup"><span data-stu-id="620f9-117">API method</span></span> |
| ------| ----- |
| <span data-ttu-id="620f9-118">创建邮件草稿</span><span class="sxs-lookup"><span data-stu-id="620f9-118">Create a message draft</span></span> | [<span data-ttu-id="620f9-119">createMessage</span><span class="sxs-lookup"><span data-stu-id="620f9-119">createMessage</span></span>](/graph/api/user-post-messages) |
| <span data-ttu-id="620f9-120">发送电子邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-120">Send an email</span></span> | [<span data-ttu-id="620f9-121">sendMail</span><span class="sxs-lookup"><span data-stu-id="620f9-121">sendMail</span></span>](/graph/api/user-sendmail) |
| <span data-ttu-id="620f9-122">答复邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-122">Reply to a message</span></span> | [<span data-ttu-id="620f9-123">回复</span><span class="sxs-lookup"><span data-stu-id="620f9-123">reply</span></span>](/graph/api/message-reply) |
| <span data-ttu-id="620f9-124">创建草稿以回复邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-124">Create a draft to reply to a message</span></span> | [<span data-ttu-id="620f9-125">createReply</span><span class="sxs-lookup"><span data-stu-id="620f9-125">createReply</span></span>](/graph/api/message-createreply) |
| <span data-ttu-id="620f9-126">对邮件执行全部答复</span><span class="sxs-lookup"><span data-stu-id="620f9-126">ReplyAll to a message</span></span> | [<span data-ttu-id="620f9-127">全部回复</span><span class="sxs-lookup"><span data-stu-id="620f9-127">replyAll</span></span>](/graph/api/message-replyall) | 
| <span data-ttu-id="620f9-128">创建草稿以全部回复邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-128">Create a draft to replyAll to a message</span></span> | [<span data-ttu-id="620f9-129">createReplyAll</span><span class="sxs-lookup"><span data-stu-id="620f9-129">createReplyAll</span></span>](/graph/api-reference/api/message-createreplyall) |
| <span data-ttu-id="620f9-130">转发邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-130">Forward a message</span></span> | [<span data-ttu-id="620f9-131">转发</span><span class="sxs-lookup"><span data-stu-id="620f9-131">forward</span></span>](/graph/api-reference/api/message-forward) |
| <span data-ttu-id="620f9-132">创建草稿以转发邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-132">Create a draft to forward a message</span></span> | [<span data-ttu-id="620f9-133">createForward</span><span class="sxs-lookup"><span data-stu-id="620f9-133">createForward</span></span>](/graph/api-reference/api/message-createforward) | 


## <a name="specify-request-header-and-mime-message-body"></a><span data-ttu-id="620f9-134">指定请求标头和 MIME 邮件正文</span><span class="sxs-lookup"><span data-stu-id="620f9-134">Specify request header and MIME message body</span></span>
<span data-ttu-id="620f9-135">可以创建 JSON 或 MIME 格式的[邮件](/graph/api-reference/v1.0/resources/message)。</span><span class="sxs-lookup"><span data-stu-id="620f9-135">You can create a [message](/graph/api-reference/v1.0/resources/message) in JSON or MIME format.</span></span> <span data-ttu-id="620f9-136">在请求标头中指定所需的格式：</span><span class="sxs-lookup"><span data-stu-id="620f9-136">Specify the intended format in the request header:</span></span>

- <span data-ttu-id="620f9-137">`Content-Type: application/json` 以在请求正文使用 JSON 格式。</span><span class="sxs-lookup"><span data-stu-id="620f9-137">`Content-Type: application/json` to use JSON format in the request body.</span></span>
- <span data-ttu-id="620f9-138">`Content-Type: text/plain` 以在请求正文使用 MIME 格式。</span><span class="sxs-lookup"><span data-stu-id="620f9-138">`Content-Type: text/plain` to use MIME format in the request body.</span></span>

<span data-ttu-id="620f9-139">以 MIME 格式指定正文时，请提供适用的 [Internet 邮件头](https://tools.ietf.org/html/rfc2076)和 [MIME 内容](https://tools.ietf.org/html/rfc2045)，并在请求正文中以 **base64** 格式对其进行编码。</span><span class="sxs-lookup"><span data-stu-id="620f9-139">When specifying the body in MIME format, provide the applicable [Internet message headers](https://tools.ietf.org/html/rfc2076) and the [MIME content](https://tools.ietf.org/html/rfc2045), and encode them in **base64** format in the request body.</span></span> <span data-ttu-id="620f9-140">Microsoft Graph 不支持单独编辑或更新 MIME 属性。</span><span class="sxs-lookup"><span data-stu-id="620f9-140">Microsoft Graph does not support editing or updating MIME properties individually.</span></span>

## <a name="example"></a><span data-ttu-id="620f9-141">示例</span><span class="sxs-lookup"><span data-stu-id="620f9-141">Example</span></span>
<span data-ttu-id="620f9-142">下面是有 Internet 邮件标头（编码前）的 MIME 内容的示例：</span><span class="sxs-lookup"><span data-stu-id="620f9-142">The following is an example of MIME content with Internet message headers (before encoding):</span></span>

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

<span data-ttu-id="620f9-143">以下是相应 base64 编码的字符串：</span><span class="sxs-lookup"><span data-stu-id="620f9-143">The following is the corresponding base64-encoded string:</span></span>

<!-- { "blockType": "ignored" } -->

```http
UmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSBieSAKY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoIHdpdGggSFRUUFM7IFRodSwgNiBNYXkgMjAyMQogMjI6NDc6MTggKzAwMDAKUmVjZWl2ZWQ6IGZyb20gY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KQogYnkgY29udG9zby5jb20gKDEwLjE5NC4yNDEuMTk3KSB3aXRoCiBTTVRQIFNlcnZlciAodmVyc2lvbj1UTFMxXzIsIApjaXBoZXI9VExTX0VDREhFX1JTQV9XSVRIX0FFU18yNTZfQ0JDX1NIQTM4NF9QMjU2KSBpZCAxNS4xLjEzNzQuMCB2aWEgTWFpbGJveDsgVGh1LCA2IE1heQogMjAyMSAyMjo0NzoxNSArMDAwMApSZWNlaXZlZDogZnJvbSBjb250b3NvLmNvbSAKKGZlODA6OjViZjo1MDU5OjRjYTA6NTAxNykgYnkgY29udG9zby5jb20gCihmZTgwOjo1YmY6NTA1OTo0Y2EwOjUwMTclMTIpIHdpdGggbWFwaSBpZCAxNS4wMS4xMzc0LjAwMDsgVGh1LCA2IE1heSAyMDIxCiAyMjo0NzoxNCArMDAwMApGcm9tOiBBZGVsZSBWYW5jZSA8QWRlbGVWQGNvbnRvc28uY29tPgpUbzogQWxleCBXaWxiZXIgPEFsZXhXQGNvbnRvc28uY29tPgpDQzogQ2hyaXN0aWUgQ2xpbmUgPENocmlzdGllQ0Bjb250b3NvLmNvbT4KU3ViamVjdDogVGhpcyBpcyBhIHRlc3QgaW4gR3JhcGggLSBNSU1FClRocmVhZC1Ub3BpYzogVGhpcyBpcyBhIHRlc3QgaW4gR3JhcGggLSBNSU1FClRocmVhZC1JbmRleDogQVFIVEpXU0hTeXdNelN6OG8wT0p1ZDQ4bkc1MEdRPT0KRGF0ZTogVGh1LCA2IE1heSAyMDIxIDIyOjQ3OjE0ICswMDAwCk1lc3NhZ2UtSUQ6Cgk8NGFhZGUyNTQ3Nzk4NDQxZWFiNTE4OGE3YTI0MzZiYzFAY29udG9zby5jb20+CkFjY2VwdC1MYW5ndWFnZTogZW4tVVMKQ29udGVudC1MYW5ndWFnZTogZW4tVVMKWC1NUy1FeGNoYW5nZS1Pcmdhbml6YXRpb24tQXV0aEFzOiBJbnRlcm5hbApYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1BdXRoTWVjaGFuaXNtOiAwNApYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1BdXRoU291cmNlOiBjb250b3NvLmNvbQpYLU1TLUhhcy1BdHRhY2g6ClgtTVMtRXhjaGFuZ2UtT3JnYW5pemF0aW9uLU5ldHdvcmstTWVzc2FnZS1JZDoKCTBmZmRiNDAyLWVjMDMtNDJjOC01ZDMyLTA4ZDRmMzdiYjUxNwpYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1TQ0w6IC0xClgtTVMtVE5FRi1Db3JyZWxhdG9yOgpYLU1TLUV4Y2hhbmdlLU9yZ2FuaXphdGlvbi1SZWNvcmRSZXZpZXdDZm1UeXBlOiAwCngtbXMtcHVibGljdHJhZmZpY3R5cGU6IEVtYWlsCngtb3JpZ2luYXRpbmctaXA6IFsxMjMuNDU2Ljc4OS4wMTJdCngtbXMtdHJhZmZpY3R5cGVkaWFnbm9zdGljOiBBU0RGRzEySEozNDU2OgpYLU1pY3Jvc29mdC1BbnRpc3BhbS1NYWlsYm94LURlbGl2ZXJ5OgoJdWNmOjA7am1yOjA7YXV0aDowO2Rlc3Q6STtFTkc6KDc1MDEyOSkoNTIwMDExMDE2KSg3MDYxNTgpKDk0NDUwNjQ1OCkoOTQ0NjI2NjA0KTsKWC1NaWNyb3NvZnQtQW50aXNwYW0tTWVzc2FnZS1JbmZvOgoJYzRVNno4NjhlZWNha1JUdFBHNzZQemlwTlJJR2w2YWZST1B3TnFHSU1zaW0wWExKaE5vV3BNNks4SzZJNjJvZ0RBalF5cFlPN3BpbmlpVmY5Sm9OWnF1N3pMY3NOUkhrZTBzcWZNYjZzeTRSanhBdzVBekZoQ0duTTJIYmN2cEJQZzhPWi94ZWNxOXd0WXdlNzFYMFJQN3lvdmFIbFlBVUcvMEo4azhmUEdGWWNKa1lHU2xWaXNqQ0ZLMzNBV3BMYm8xb1luRVdlaUtncTU2ZE96QXdSTnVpNzhsNHRQdzBrSW9mYWZnRXBkbnlnekdLYkF1WGkxWXE5T0FCRUNkYzBqRUNjY1VmMUREMFZaVk5sdDE3eHFDUE5UaTYzay9YYkpwUUM2aXdwMHRuSnhJZUhmWjJweG1WdkZGYnJDYWgvamRmTlpTdkN3WkdWNWNqbEFMUWFiYWZacW1mU1VtZW85Nmx4Nks4cHBBOUlVd2hUV3REYkhpTXorU1BxWDBmeUZDbVlSNDlaYktFRnlKanRoODdqU2MwejJPbGNSZC8vV0tySFBJeFZxSEJqbFJEWTJ1M08vOFNreXhOY1ZxcXVsRm5vQ011UjF3ZXFDSzJQYXBkUGJqMllMN0FzWnJNNms0SENnblgvVzZ6NGhGYnlsWkNiUlpUczZBWFJPbSt5VDN1bEdobENja0lLL2ZmNHZFVFRzZksyT3lVREoraGc1NVFWdE81Nit1Y1g1d1hqdDVYazVWZisxQlZTTVNuRzYxVEtKd1hHV21RWnArdTQvc1YrN1k5VzIwZTlWUFNBL1NnWkhOTVVSRXNSbWtBSWs4VURkVHdGTU53SEpHYQpDb250ZW50LVR5cGU6IG11bHRpcGFydC9hbHRlcm5hdGl2ZTsKCWJvdW5kYXJ5PSJfMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfIgpNSU1FLVZlcnNpb246IDEuMAoKLS1fMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfCkNvbnRlbnQtVHlwZTogdGV4dC9wbGFpbjsgY2hhcnNldD0iaXNvLTg4NTktMSIKQ29udGVudC1UcmFuc2Zlci1FbmNvZGluZzogcXVvdGVkLXByaW50YWJsZQoKSGVsbG8gQWxleCwKCldlIGFyZSB0ZXN0aW5nIHRoZSBHcmFwaCBNSU1FIGZlYXR1cmUuCgpLaW5kIHJlZ2FyZHMsCgpBZGVsZQoKLS1fMDAwX01OMlBSMTNNQjMxNTJCNUZDQTk5MTJCRUEyRTQ5MDE4OUQ1NTg5TU4yUFIxM01CMzE1Mm5hbXBfCkNvbnRlbnQtVHlwZTogdGV4dC9odG1sOyBjaGFyc2V0PSJpc28tODg1OS0xIgpDb250ZW50LVRyYW5zZmVyLUVuY29kaW5nOiBxdW90ZWQtcHJpbnRhYmxlCgo8aHRtbD4KPGhlYWQ+CjxtZXRhIGh0dHAtZXF1aXY9M0QiQ29udGVudC1UeXBlIiBjb250ZW50PTNEInRleHQvaHRtbDsgY2hhcnNldD0zRGlzby04ODU5LT0KMSI+CjxzdHlsZSB0eXBlPTNEInRleHQvY3NzIiBzdHlsZT0zRCJkaXNwbGF5Om5vbmU7Ij4gUCB7bWFyZ2luLXRvcDowO21hcmdpbi1ibz0KdHRvbTowO30gPC9zdHlsZT4KPC9oZWFkPgo8Ym9keSBkaXI9M0QibHRyIj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KSGVsbG8gQWxleCwmbmJzcDs8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KPGJyPgo8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KV2UgYXJlIHRlc3RpbmcgdGhlIEdyYXBoIE1JTUUgZmVhdHVyZS4mbmJzcDs8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KPGJyPgo8L2Rpdj4KPGRpdiBzdHlsZT0zRCJmb250LWZhbWlseTogQ2FsaWJyaSwgQXJpYWwsIEhlbHZldGljYSwgc2Fucy1zZXJpZjsgZm9udC1zaXplPQo6IDEycHQ7IGNvbG9yOiByZ2IoMCwgMCwgMCk7Ij4KS2luZCByZWdhcmRzLDwvZGl2Pgo8ZGl2IHN0eWxlPTNEImZvbnQtZmFtaWx5OiBDYWxpYnJpLCBBcmlhbCwgSGVsdmV0aWNhLCBzYW5zLXNlcmlmOyBmb250LXNpemU9CjogMTJwdDsgY29sb3I6IHJnYigwLCAwLCAwKTsiPgo8YnI+CjwvZGl2Pgo8ZGl2IHN0eWxlPTNEImZvbnQtZmFtaWx5OiBDYWxpYnJpLCBBcmlhbCwgSGVsdmV0aWNhLCBzYW5zLXNlcmlmOyBmb250LXNpemU9CjogMTJwdDsgY29sb3I6IHJnYigwLCAwLCAwKTsiPgpBZGVsZTwvZGl2Pgo8L2JvZHk+CjwvaHRtbD4KCi0tXzAwMF9NTjJQUjEzTUIzMTUyQjVGQ0E5OTEyQkVBMkU0OTAxODlENTU4OU1OMlBSMTNNQjMxNTJuYW1wXy0t

```

<span data-ttu-id="620f9-144">如果要包括文件附件，请将采用 base64 的文件元数据和`Content-Transfer-Encoding`标头附加到 MIME内 容中：</span><span class="sxs-lookup"><span data-stu-id="620f9-144">To include a file attachment, append the file metadata and `Content-Transfer-Encoding` header in base64 to the MIME content:</span></span>

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

## <a name="error-conditions-and-messages"></a><span data-ttu-id="620f9-145">错误条件和邮件</span><span class="sxs-lookup"><span data-stu-id="620f9-145">Error conditions and messages</span></span>

|<span data-ttu-id="620f9-146">应用场景</span><span class="sxs-lookup"><span data-stu-id="620f9-146">Scenario</span></span>|<span data-ttu-id="620f9-147">操作</span><span class="sxs-lookup"><span data-stu-id="620f9-147">Operation</span></span>|<span data-ttu-id="620f9-148">错误代码</span><span class="sxs-lookup"><span data-stu-id="620f9-148">Error code</span></span>|<span data-ttu-id="620f9-149">错误消息</span><span class="sxs-lookup"><span data-stu-id="620f9-149">Error message</span></span>|
|--------|------|----|-------|
| <span data-ttu-id="620f9-150">MIME 内容格式错误、丢失</span><span class="sxs-lookup"><span data-stu-id="620f9-150">MIME content malformed, missing</span></span> | <span data-ttu-id="620f9-151">POST, PUT</span><span class="sxs-lookup"><span data-stu-id="620f9-151">POST, PUT</span></span> | <span data-ttu-id="620f9-152">400</span><span class="sxs-lookup"><span data-stu-id="620f9-152">400</span></span> | <span data-ttu-id="620f9-153">MIME 内容无效的 base64 字符串。</span><span class="sxs-lookup"><span data-stu-id="620f9-153">Invalid base64 string for MIME content.</span></span> |


