---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbcaa38cd7a8c14f02c4dad3d46ea4d3e87810a3f6d0bcf1926cd8f326e360a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleSetting = {
   adminEligibleSettings: [
      {
         ruleIdentifier: 'ExpirationRule',
         setting: '{\"permanentAssignment\':false,\'maximumGrantPeriodInMinutes\':129600}"
      }
   ]
};

await client.api('/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5')
    .version('beta')
    .update(governanceRoleSetting);

```