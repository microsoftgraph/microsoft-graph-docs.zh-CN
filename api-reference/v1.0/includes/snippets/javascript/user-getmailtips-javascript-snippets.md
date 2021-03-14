---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f02e701a4fbdd0e065e263e1d0d3b419fbd818e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailTips = {
    EmailAddresses: [
        'danas@contoso.onmicrosoft.com', 
        'fannyd@contoso.onmicrosoft.com'
    ],
    MailTipsOptions: 'automaticReplies, mailboxFullStatus'
};

await client.api('/me/getMailTips')
    .post(mailTips);

```