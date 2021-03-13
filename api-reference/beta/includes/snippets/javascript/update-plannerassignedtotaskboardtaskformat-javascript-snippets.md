---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 917bf41197eaba6caccfed01556fa5d9eef37178
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802301"
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