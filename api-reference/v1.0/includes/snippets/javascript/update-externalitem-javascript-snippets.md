---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d8c44bf51b7be5b25b03965d5d79077c2112645f
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: 'everyone',
      value: '67a141d8-cf4e-4528-ba07-bed21bfacd2d',
      accessType: 'grant'
    }
  ]
};

await client.api('/external/connections/contosohr/items/TSP228082938')
    .update(externalItem);

```