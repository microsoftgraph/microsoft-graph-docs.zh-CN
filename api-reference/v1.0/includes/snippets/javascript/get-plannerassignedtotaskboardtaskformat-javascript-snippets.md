---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cfcf5ab97797aba8b69ca61ce229138203bd3f2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerAssignedToTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .get();

```