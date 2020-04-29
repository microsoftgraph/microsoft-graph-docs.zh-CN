---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bba7fad557ac49a141a0a45301fa42b39a5e163
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935181"
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
      value: "49103559-feac-4575-8b94-254814dfca72",
      accessType: "deny",
      identitySource: "Azure Active Directory"
    }
  ],
  properties: {
    title: "Error in the payment gateway",
    priority: 1,
    assignee: "john@contoso.com"
  },
  content: {
    value: "<h1>Error in payment gateway</h1><p>Error details...</p>",
    type: "html"
  }
};

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .put(externalItem);

```