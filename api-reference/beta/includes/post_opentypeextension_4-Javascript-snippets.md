---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 06a012c904bfa6ea8676ed14279b1b97b9cfbc96
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "html",
      content: "<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>"
    },
  extensions: [
    {
      @odata.type: "microsoft.graph.openTypeExtension",
      extensionName: "Com.Contoso.HR",
      companyName: "Contoso",
      expirationDate: "2015-07-03T13:04:00.000Z",
      topPicks: [
        "Employees only",
        "Add spouse or guest",
        "Add family"
      ]
    }
  ]
  }
};

let res = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply')
    .version('beta')
    .post(reply);

```