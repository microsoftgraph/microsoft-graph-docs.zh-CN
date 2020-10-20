---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06a012c904bfa6ea8676ed14279b1b97b9cfbc96
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613876"
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