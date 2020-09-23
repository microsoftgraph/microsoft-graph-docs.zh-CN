---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ab9dd97e99478fc238c1483b7be6b0e028170e4
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230692"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  @odata.type: "microsoft.graph.externalItem",
  acl: [
    {
      type: "user",
      value: "e811976d-83df-4cbd-8b9b-5215b18aa874",
      accessType: "grant",
      identitySource: "azureActiveDirectory"
    },
    {
      type: "group",
      value: "14m1b9c38qe647f6a",
      accessType: "deny",
      identitySource: "external"
    }
  ],
  properties: {
    title: "Error in the payment gateway",
    priority: 1,
    assignee: "john@contoso.com"
  },
  content: {
    value: "Error in payment gateway...",
    type: "text"
  }
};

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .put(externalItem);

```