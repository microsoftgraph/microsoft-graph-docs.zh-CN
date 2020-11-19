---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: cb404fe9d0e4f592bcbc5932a5900c82084401b8
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const stringKeyStringValuePair = Content-Type: application/json
Content-length: 122

{
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