---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bfd7f152957d6da2641885a1103e69a6c7f91db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798106"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
  assignedLabels: 
  [
    {
        labelId: '45cd0c48-c540-4358-ad79-a3658cdc5b88'
    }
  ]
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```