---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: baebcbd7665fbba4861da18eec2db39ca8754ba9
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687467"
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
    .post(subjectRightsRequest);

```