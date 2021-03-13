---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a371c8ec736b0a0e1bb46ad2fd6b89e3e85a994
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782158"
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