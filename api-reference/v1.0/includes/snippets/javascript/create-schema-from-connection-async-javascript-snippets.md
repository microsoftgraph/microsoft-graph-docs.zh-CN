---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4eab45540120f3a93eab577cd8c8995970743f88518c6aff1a3b2eab4040d6e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schema = {
  baseType: 'microsoft.graph.externalItem',
  properties: [
    {
      name: 'ticketTitle',
      type: 'String',
      isSearchable: 'true',
      isRetrievable: 'true',
      labels: [
        'title'
      ]
    },
    {
      name: 'priority',
      type: 'String',
      isQueryable: 'true',
      isRetrievable: 'true',
      isSearchable: 'false'
    },
    {
      name: 'assignee',
      type: 'String',
      isRetrievable: 'true'
    }
  ]
};

await client.api('/external/connections/contosohr/schema')
    .post(schema);

```