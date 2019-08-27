---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 75fde72d78e72e8a629dee3bb9fbdad8748be94f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636501"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleSetting = {
   adminEligibleSettings:[
      {
         ruleIdentifier:"ExpirationRule",
         setting:{\"permanentAssignment\:false,\maximumGrantPeriodInMinutes\:129600}"
      }
   ]
};

let res = await client.api('/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5')
    .version('beta')
    .update(governanceRoleSetting);

```