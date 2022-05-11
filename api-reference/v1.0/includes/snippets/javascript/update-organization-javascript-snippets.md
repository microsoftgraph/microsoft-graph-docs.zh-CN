---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade7676cd9585085a8288584b083ad26ebd7f170
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327220"
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

await client.api('/organization/84841066-274d-4ec0-a5c1-276be684bdd3')
    .update(organization);

```