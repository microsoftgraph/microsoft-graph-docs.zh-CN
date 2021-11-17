---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b773179ec346dd9aa10c657c0ad04f032908d1d959e1de702edc2e716f2a69d0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: 'String',
  closedDateTime: 'String (timestamp)',
  comments: ['String'],
  feedback: '@odata.type: microsoft.graph.alertFeedback',
  status: '@odata.type: microsoft.graph.alertStatus',
  tags: ['String'],
  vendorInformation: 
    {
      provider: 'String',
      vendor: 'String'
    }
};

await client.api('/security/alerts/{alert_id}')
    .version('beta')
    .update(alert);

```