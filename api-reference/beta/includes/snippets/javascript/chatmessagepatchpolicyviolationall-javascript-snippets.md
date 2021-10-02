---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aef30011eac4b61d87d757e0d49855bf4ccef43f2422c4bee174e08883369567
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  policyViolation: {
    policyTip: {
      generalText: 'This item has been blocked by the administrator.',
      complianceUrl: 'https://contoso.com/dlp-policy-page',
      matchedConditionDescriptions: ['Credit Card Number']
    },
    verdictDetails: 'AllowOverrideWithoutJustification,AllowFalsePositiveOverride',
    dlpAction: 'BlockAccess'
  }
};

await client.api('/teams/e1234567-e123-4276-55555-6232b0e3a89a/channels/a7654321-e321-0000-0000-123b0e3a00a/messages/19:a21b0b0c05194ebc9e30000000000f61@thread.skype')
    .version('beta')
    .update(chatMessage);

```