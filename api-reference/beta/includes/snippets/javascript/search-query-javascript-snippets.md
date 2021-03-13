---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3df15ce3a6b3a311bd2c4e3131847225c52588a5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808081"
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
        'externalItem'
      ],
      contentSources: [
        '/external/connections/connectionfriendlyname'
      ],
      query: {
        queryString: 'contoso product'
      },
      from: 0,
      size: 25,
      fields: [
        'title',
        'description'
      ]
    }
  ]
};

await client.api('/search/query')
    .version('beta')
    .post(searchResponse);

```