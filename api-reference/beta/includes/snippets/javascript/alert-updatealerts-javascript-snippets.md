---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f5ef6c61ff85651fb19925d2d9a58a3974f0e03543b8d74dd0c814285ed8225
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215730"
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