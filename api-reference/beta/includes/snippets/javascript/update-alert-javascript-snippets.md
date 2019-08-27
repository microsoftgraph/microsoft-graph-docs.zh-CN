---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82de0fe34d3ff6df39fad1c383868cdd9c5e8796
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const alert = {
  assignedTo: "String",
  closedDateTime: "String (timestamp)",
  comments: ["String"],
  feedback: "@odata.type: microsoft.graph.alertFeedback",
  status: "@odata.type: microsoft.graph.alertStatus",
  tags: ["String"],
  vendorInformation:
    {
      provider: "String",
      vendor: "String"
    }
};

let res = await client.api('/security/alerts/{alert_id}')
    .version('beta')
    .update(alert);

```