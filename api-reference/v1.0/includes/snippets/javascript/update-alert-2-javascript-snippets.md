---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 583a2b5f6345e4803ddcaec5501ce952316244da89fa17efc602d90daa901e88
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: 'String',
  closedDateTime: 'String (timestamp)',
  comments: [
    'String'
  ],
  feedback: '@odata.type: microsoft.graph.alertFeedback',
  status: '@odata.type: microsoft.graph.alertStatus',
  tags: [
    'String'
  ],
  vendorInformation: {
    provider: 'String',
    vendor: 'String'
  }
};

await client.api('/security/alerts/{alert_id}')
    .update(alert);

```