---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7fde94a6613d39fc44b51fd9775132d86b267282
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734823"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .get();

```