---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7eb4bf092355bcaeae6d8d10e97623ac8fd4d12
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336086"
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
      type: 'string',
      isSearchable: 'true',
      isRetrievable: 'true',
      labels: [
        'title'
      ]
    },
    {
      name: 'priority',
      type: 'string',
      isQueryable: 'true',
      isRetrievable: 'true',
      isSearchable: 'false'
    },
    {
      name: 'assignee',
      type: 'string',
      isRetrievable: 'true'
    }
  ]
};

await client.api('/external/connections/contosohr/schema')
    .version('beta')
    .update(schema);

```