---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c63037e8510c59297ea04341ff491b6175a617bd6bd05016b08dd4494484d56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221224"
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

await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat')
    .version('beta')
    .update(plannerAssignedToTaskBoardTaskFormat);

```