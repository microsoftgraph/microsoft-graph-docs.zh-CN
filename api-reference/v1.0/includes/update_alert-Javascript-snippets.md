---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4637ebae11553452568e67ce8f0459309585e484
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: "String",
  closedDateTime: "String (timestamp)",
  comments: [
    "String"
  ],
  feedback: "@odata.type: microsoft.graph.alertFeedback",
  status: "@odata.type: microsoft.graph.alertStatus",
  tags: [
    "String"
  ],
  vendorInformation: {
    provider: "String",
    vendor: "String"
  }
};

let res = await client.api('/security/alerts/{alert_id}')
    .update({alert : alert});

```