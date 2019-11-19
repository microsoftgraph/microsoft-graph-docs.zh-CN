---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30cc89803eeae39663ec94ff715b3918177f3baf
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37996385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const searchResponse = {
  requests: [
    {
      entityTypes: [
        "microsoft.graph.externalItem"
      ],
      contentSources: [
        "/external/connections/connectionfriendlyname"
      ],
      query: {
        query_string: {
          query: "contoso product"
        }
      },
      from: 0,
      size: 25,
      stored_fields: [
        "title",
        "description"
      ]
    }
  ]
};

let res = await client.api('/search/query')
    .version('beta')
    .post(searchResponse);

```