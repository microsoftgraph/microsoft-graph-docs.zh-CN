---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f655dc44ca07b32604aef3446e631ca3755fb1a5
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580748"
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

await client.api('/connections/contosohr/items/TSP228082938')
    .update(externalItem);

```