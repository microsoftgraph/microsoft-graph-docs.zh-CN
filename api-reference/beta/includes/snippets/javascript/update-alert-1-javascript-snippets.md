---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbb299faab47eeebddbeb235ea98217e35d68e37
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942815"
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