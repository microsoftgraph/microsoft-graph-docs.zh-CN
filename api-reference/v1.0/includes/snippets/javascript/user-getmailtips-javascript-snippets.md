---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 80ca423f95fa747ee9af2b13a77ec164d1e71833
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailTips = {
    EmailAddresses: [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    MailTipsOptions: "automaticReplies, mailboxFullStatus"
};

let res = await client.api('/me/getMailTips')
    .post(mailTips);

```