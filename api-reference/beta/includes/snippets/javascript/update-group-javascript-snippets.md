---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b83aafe0407a288c5c523153390d02ba24192a8
ms.sourcegitcommit: 43f7800894857a29f02fffaf4a50ad6386b5bf59
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44524489"
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
        "labelId" : "45cd0c48-c540-4358-ad79-a3658cdc5b88"
    }
  ]
};

let res = await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```