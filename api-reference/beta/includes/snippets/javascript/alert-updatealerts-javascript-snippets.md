---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 275fb3eebe95efd09ad356ea1c89ddfb23c66299
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  value: [
    {
      assignedTo: 'String',
      closedDateTime: 'String (timestamp)',
      comments: ['String'],
      feedback: {'@odata.type': 'microsoft.graph.alertFeedback'},
      id: 'String (identifier)',
      status: {'@odata.type': 'microsoft.graph.alertStatus'},
      tags: ['String'],
      vendorInformation: 
        {
          provider: 'String',
          vendor: 'String'
        }
    }
  ]
};

await client.api('/security/alerts/updateAlerts')
    .version('beta')
    .post(alert);

```