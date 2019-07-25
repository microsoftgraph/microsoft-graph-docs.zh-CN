---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5e14eb8b568b26fb1a931d86bc40fd340358fe3c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716600"
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
    .version('beta')
    .post(mailTips);

```