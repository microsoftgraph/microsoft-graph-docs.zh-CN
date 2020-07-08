---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e3b538f8922b3a9f28e59bcd1d5a5b7359b00d5
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schema = {
  baseType: "microsoft.graph.externalItem",
  properties: [
    {
      name: "ticketTitle",
      type: "String",
      isSearchable: "true",
      isRetrievable: "true",
      labels: [
        "title"
      ]
    },
    {
      name: "priority",
      type: "String",
      isQueryable: "true",
      isRetrievable: "true",
      isRefinable: "true",
      isSearchable: "false"
    },
    {
      name: "assignee",
      type: "String",
      isRetrievable: "true"
    }
  ]
};

let res = await client.api('/external/connections/contosohr/schema')
    .version('beta')
    .post(schema);

```