---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5d9827f20e3b74fc3b241d4a088a91211f9c9af
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stringKeyStringValuePair = {
    parameters: [{
      subjects: [{
          objectId: '9bb0f679-a883-4a6f-8260-35b491b8b8c8',
          objectTypeName: 'User'
      }],
      ruleId: 'ea807875-5618-4f0a-9125-0b46a05298ca'
    }]
  };

await client.api('/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand')
    .version('beta')
    .post(stringKeyStringValuePair);

```