---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a0b28aee8ac4235f7183251510227fb3409e3a4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stringKeyStringValuePair = Content-Type: application/json
Content-length: 122

{
    "parameters" [{
      subjects: [{
          objectId: "9bb0f679-a883-4a6f-8260-35b491b8b8c8",
          objectType: "User"
      }],
      ruleId: "ea807875-5618-4f0a-9125-0b46a05298ca"
    }]
  };

let res = await client.api('/servicePrincipals/{servicePrincipalsId}/synchronization/jobs/{synchronizationJobId}/provisionOnDemand')
    .version('beta')
    .post(stringKeyStringValuePair);

```