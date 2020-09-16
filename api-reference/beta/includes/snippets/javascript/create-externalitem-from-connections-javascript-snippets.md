---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 031e6b0b1ade5820619084e52a9c174b46e32f50
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938466"
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
      identitySource: "azureActiveDirectory"
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