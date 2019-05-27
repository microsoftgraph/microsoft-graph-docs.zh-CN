---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9015dee19666073313d47d4da183822a546d26f8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462318"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organization = {
  "marketingNotificationEmails" : ["marketing@contoso.com"],
  "privacyProfile" :
    {
      contactEmail:"alice@contoso.com",
      statementUrl:"https://contoso.com/privacyStatement"
    },
  "securityComplianceNotificationMails" : ["security@contoso.com"],
  "securityComplianceNotificationPhones" : ["(123) 456-7890"],
  "technicalNotificationMails" : ["tech@contoso.com"]
};

let res = await client.api('/organization/{id}')
    .update({organization : organization});

```