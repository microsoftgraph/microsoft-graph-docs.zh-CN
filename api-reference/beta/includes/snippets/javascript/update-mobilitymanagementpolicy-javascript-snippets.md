---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a74e2d230b9935e9809d1efd986c878f716544cf
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368852"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mobilityManagementPolicy = {
  '@odata.type': '#microsoft.graph.mobilityManagementPolicy',
  complianceUrl: 'https://portal.mg.contoso.com/?portalAction=Compliance',
  discoveryUrl: 'https://enrollment.mg.contoso.com/enrollmentserver/discovery.svc',
  termsOfUseUrl: 'https://portal.mg.contoso.com/TermsofUse.aspx'
};

await client.api('/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020')
    .version('beta')
    .update(mobilityManagementPolicy);

```