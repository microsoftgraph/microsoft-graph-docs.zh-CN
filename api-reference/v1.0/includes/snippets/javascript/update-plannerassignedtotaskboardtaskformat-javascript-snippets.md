---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 189c3210f580fd5469fadf0810313cb11e34223fcc80c3691764b451577b652b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277871"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerAssignedToTaskBoardTaskFormat = {
  orderHintsByAssignee: {
    'aaa27244-1db4-476a-a5cb-004607466324': '8566473P 957764Jk!'
  }
};

await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .update(plannerAssignedToTaskBoardTaskFormat);

```