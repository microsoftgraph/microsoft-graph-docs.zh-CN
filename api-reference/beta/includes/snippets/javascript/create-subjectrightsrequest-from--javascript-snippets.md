---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a4eec20f7a0d43732eaac3613919b6cfbc1e5d1
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561792"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const subjectRightsRequest = {
    type: 'microsoft.graph.subjectRightsRequestType',
    dataSubjectType: 'microsoft.graph.dataSubjectType',
    regulations: ['String'],
    displayName: 'String',
    description: 'String',
    internalDueDateTime: 'String (timestamp)',
    dataSubject: {
        firstName: 'String',
        lastName: 'String',
        email: 'String',
        residency: 'String',
        phoneNumber: 'String',
        SSN: 'String'
    }
};

await client.api('/privacy/subjectRightsRequests')
    .version('beta')
    .post(subjectRightsRequest);

```