---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5bfd7f152957d6da2641885a1103e69a6c7f91db
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944245"
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