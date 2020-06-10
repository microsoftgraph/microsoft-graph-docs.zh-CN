---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea1a4f45a32208cd910db52bc1b64409b26eb73a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685093"
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
        "externalItem"
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