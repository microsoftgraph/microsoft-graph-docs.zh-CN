---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dbb88784eed0d05a66a2bd7e0e502d0358637887
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729119"
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
    .version('beta')
    .update({organization : organization});

```