---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 934bd8ac7b51f9314598ef25a94aab917cccc08c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const organization = {
  marketingNotificationEmails: ['marketing@contoso.com'],
  privacyProfile: 
    {
      contactEmail: 'alice@contoso.com',
      statementUrl: 'https://contoso.com/privacyStatement'
    },
  securityComplianceNotificationMails: ['security@contoso.com'],
  securityComplianceNotificationPhones: ['(123) 456-7890'],
  technicalNotificationMails: ['tech@contoso.com']
};

await client.api('/organization/{id}')
    .update(organization);

```