---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7fde94a6613d39fc44b51fd9775132d86b267282
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .get();

```