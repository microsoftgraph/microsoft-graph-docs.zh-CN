---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b38119d2295410d1fdf0dbcf3ea106d36fab805
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mobilityManagementPolicy = {
  '@odata.type': '#microsoft.graph.mobilityManagementPolicy',
  complianceUrl: 'https://portal.uem.contoso.com/?portalAction=Compliance',
  discoveryUrl: 'https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc',
  termsOfUseUrl: 'https://portal.uem.contoso.com/TermsofUse.aspx'
};

await client.api('/policies/mobileDeviceManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020')
    .version('beta')
    .update(mobilityManagementPolicy);

```