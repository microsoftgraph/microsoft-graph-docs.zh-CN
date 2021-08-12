---
title: 获取邮件的 MIME 内容
description: 多用途 Internet 邮件扩展 (MIME) 是一种行业电子邮件标准。 你现在可以使用 `$value` 段来获取 Outlook 邮件的 MIME 内容。
author: abheek-das
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: ff2724f5dd2f9325d53e5a7506887f944ba350e96d592be778e46b5c8e2dc67a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126051"
---
# <a name="get-mime-content-of-a-message"></a>获取邮件的 MIME 内容

MIME 是一种行业电子邮件标准。 许多电子邮件应用程序以 MIME 格式创建邮件并将其保存在扩展名为 .EML 的文件中。 

即使 Outlook _不_ 以 MIME 格式保存邮件，也有两种方法可以获得 MIME 格式的 Outlook 邮件正文：

- 你可以将 `$value` 段附加到该邮件的 get-message 操作。
- 如果邮件附加到 Outlook 项目或组帖子，则可以将 `$value` 段附加到该项目或组帖子的 get-attachment 操作。

在任何一种情况下，你的应用都必须具有访问 Outlook 项目或组帖子的相应[权限](permissions-reference.md#mail-permissions)才能应用 get-message 或 get-attachment 操作。 

然后，你可以将邮件正文内容保存在 .EML 文件中，并将该文件附加到企业系统中的记录，例如 CRM、ERP 和错误跟踪的记录。 


## <a name="what-is-mime"></a>什么是 MIME？

MIME 是 Internet 电子邮件用于通过 SMTP 传输以下类型内容的标准： 

- 纯文本邮件
- 带有可选内容（即，纯文本和 HTML）邮件
- 回复邮件附上原始邮件
- 带有图像、音频、视频或应用程序文件附件的文本邮件  
- 其他邮件构造

以下是邮件中的典型 MIME 标头。 有关详细信息，请参阅 [RFC 2045](https://tools.ietf.org/html/rfc2045)。

- `MIME-Version` - 指示邮件是 MIME 格式的。
- `Content-Type` - 指示邮件或邮件的一部分的媒体类型，由 *类型* 和 *子类型* 表示。 它还包括一个 `boundary` 字段，该字段将字符串指定为 MIME 边界或封装边界，具体取决于 `Content-Type` 的位置。 
- `Content-Disposition` - 提供附件的详细信息，例如其演示样式（`inline` 或 `attachment`）、文件名、创建日期和上次修改日期。
- `Content-Transfer-Encoding` - 指定表示二进制数据的编码方法。

## <a name="get-mime-content-of-an-outlook-message"></a>获取 Outlook 邮件的 MIME 内容

你可以通过在[获取邮件](/graph/api/message-get?view=graph-rest-1.0)时附加 `$value` 段来获取邮件的 MIME 表示： 

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/$value
```

### <a name="example"></a>示例

以下是请求使用其 MIME 内容返回登录用户邮箱中的邮件的示例。

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

以下是答复。 MIME 内容以 `MIME-Version` 标头开头。 

<!-- { "blockType": "ignored" } -->
```http
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 
x-ms-publictraffictype: Emai

```http
MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```

## <a name="get-mime-content-of-an-outlook-message-attached-to-an-outlook-item-or-group-post"></a>获取附加到 Outlook 项目或组帖子的 Outlook 邮件的 MIME 内容

你还可以获取 Outlook 邮件的 MIME 表示，如果邮件附加到 Outlook [事件](/graph/api/resources/event?view=graph-rest-1.0)、[邮件](/graph/api/resources/message?view=graph-rest-1.0)、[任务](/graph/api/resources/outlooktask?view=graph-rest-beta)或组[帖子](/graph/api/resources/post?view=graph-rest-1.0)，你的应用程序可以访问。

为此，标识邮件附件，并在[获取该附件](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment
)时附加 `$value` 段。 以下显示了访问附件的一些常用方法。 有关详细信息，请参阅[获取附件](/graph/api/attachment-get?view=graph-rest-1.0#http-request)。

如果邮件附加到用户默认日历中的事件：
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/attachments/{id}/$value
```

如果邮件附加到用户邮箱中的其他邮件：
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/attachments/{id}/$value
```

如果邮件附加到用户默认任务文件夹中的 Outlook 任务：
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

如果邮件附加到指定的组帖子：
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

### <a name="example"></a>示例

以下是获取已附加到另一封邮件的邮件，并以 MIME 格式返回正文的示例。

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUAAA7XW-lAAA=/attachments/AAMkAGUAAA7XW-lAAABEgAQAFBZJBq4EN5FlCSvNV-M-FI=/$value
```

以下是答复。 MIME 内容以 `MIME-Version` 标头开头。 

<!-- { "blockType": "ignored" } -->
```http
Received: from MWHPR22MB0302.namprd22.prod.outlook.com (2603:10b6:104:5::23)
 by MWHPR2201MB1053.namprd22.prod.outlook.com with HTTPS via
 CO2PR04CA0193.NAMPRD04.PROD.OUTLOOK.COM; Mon, 22 Apr 2019 19:48:20 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com (10.172.167.21) by
 MWHPR22MB0302.namprd22.prod.outlook.com (10.173.53.146) with Microsoft SMTP
 Server (version=TLS1_2, cipher=TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384) id
 15.20.1813.12; Mon, 22 Apr 2019 19:48:16 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc]) by MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc%9]) with mapi id 15.20.1813.017; Mon, 22 Apr 2019
 19:48:16 +0000
From: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
To: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
Subject: Press conference
Thread-Topic: Press conference
Thread-Index: AQHU+UQNzFWFTilRjECtpiWorLYxqA==
Date: Mon, 22 Apr 2019 19:48:16 +0000
Message-ID:
    <MWHPR22MB100769D1513B3DC0F007B2ECD4220@MWHPR22MB1007.namprd22.prod.outlook.com>
Accept-Language: en-US
Content-Language: en-US
X-MS-Exchange-Organization-AuthAs: Internal
X-MS-Exchange-Organization-AuthMechanism: 04
X-MS-Exchange-Organization-AuthSource: MWHPR22MB1007.namprd22.prod.outlook.com
X-MS-Has-Attach:
X-MS-Exchange-Organization-Network-Message-Id:
    88bed46b-a860-40fb-591e-08d6c75b76c1
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
x-ms-publictraffictype: Email
authentication-results: contoso.OnMicrosoft.com; dkim=none (message not
 signed) header.d=none;contoso.OnMicrosoft.com; dmarc=none action=none
 header.from=contoso.OnMicrosoft.com;
x-originating-ip: [2001:4898:80e8:9:9607:7cf8:4576:961c]
x-ms-office365-filtering-correlation-id: 88bed46b-a860-40fb-591e-08d6c75b76c1
x-microsoft-antispam:
    BCL:0;PCL:0;RULEID:(2390118)(7020095)(4652040)(7021145)(8989299)(4534185)(7022145)(4603075)(4627221)(201702281549075)(8990200)(5600141)(711020)(4605104)(2017052603328)(7177060)(7171020)(7173020)(7193020);SRVR:MWHPR22MB0302;
x-ms-traffictypediagnostic: MWHPR22MB0302:
X-Microsoft-Antispam-Mailbox-Delivery:
    ucf:0;jmr:0;ex:0;auth:0;dest:I;ENG:(750119)(520011016)(706158)(944506303)(944626516);
X-Microsoft-Antispam-Message-Info:
    twccJ5SmB7ZvueSjaTBdmtD3489zlRiHPqiO3DBEil1jBx5xhl/5G/fK2GLgdH0klkE2uoUAAvdvpmxiJezwxCtmn11Nq3kvaOuypDL2TDVdYvWkTfSt4SYfVTp34iBoDlvOEbTh8LTl5J/dz98cgvoRdiE7TUJBXTGvUyVTQX1LG7Xg1hNXMu6XLng6Axdn/ka2NUhmzOa3hEl9yoUI8g3G66Vq3zzVRQFpS+P5+/d1LcbKHsuYMgZNBzBeM6dLnMnwOH9rKXqjV+d72YDnQw4SkbULkoEsQs2Vq0e4URDtkzQwHqcoPv1W2HE4pypmiqkl4M6lJtBccF3MWPP/xNxl6NL5gLSpZCILbg8gQ1UxxX8Kdhd4KWbDa3ayHLHBr11hMNFbGftcUZbZ6jrAtiIGYtGzaAxHqlYC3lUHXZIMdygT76enIJJwklQ1VIp4
Content-Type: multipart/alternative;
    boundary="_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_"
MIME-Version: 1.0

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/plain; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

The press conference will be on May 15. We arranged to have the press gathe=
r at 2pm outside the main entrance.

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/html; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

<html>
<head>
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-=
1">
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi=
n-bottom:0;} --></style>
</head>
<body dir=3D"ltr">
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font=
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr">
<p style=3D"margin-top:0;margin-bottom:0">The press conference will be on M=
ay 15. We arranged to have the press gather at 2pm outside the main entranc=
e.</p>
</div>
</body>
</html>

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_--
```

## <a name="next-steps"></a>后续步骤

详细了解以下信息：

- 获取事件、邮件、Outlook 任务或组帖子的[项目附件的 MIME 内容](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment)
- [为什么与 Outlook 邮件集成](outlook-mail-concept-overview.md)
- [使用功能邮件 API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) 及其在 Microsoft Graph v1.0 中的[用例](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)
