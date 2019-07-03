---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7d364c6bbca882d937960af1d53b3d519a85c8bd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520131"
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
    .update({alert : alert});

```