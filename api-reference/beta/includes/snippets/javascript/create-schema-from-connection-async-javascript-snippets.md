---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a0be5918145f7b5471039eb8a80e045dd83eec2
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938445"
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