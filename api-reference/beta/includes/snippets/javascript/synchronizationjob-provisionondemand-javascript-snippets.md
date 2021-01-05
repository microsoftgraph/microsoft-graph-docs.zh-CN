---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5ca20cb642b4c52a413fa72a57957a09b3e619c
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753412"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stringKeyStringValuePair = {
    parameters: [{
      subjects: [{
          objectId: "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          objectTypeName: "User"
      }],
      ruleId: "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  };

let res = await client.api('/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand')
    .version('beta')
    .post(stringKeyStringValuePair);

```