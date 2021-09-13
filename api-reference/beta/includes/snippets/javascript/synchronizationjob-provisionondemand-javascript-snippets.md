---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b01ba512e0e5d48ee518f113d5bfa58c019c4987da74d7a4baa58addf9f15c8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220203"
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