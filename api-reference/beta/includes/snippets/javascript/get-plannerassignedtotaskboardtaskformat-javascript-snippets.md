---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 440edd1dc2b9c6f3948f1df25f1f6a1fb9d13e5b1bc4e797ab288e68d6e1c013
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerAssignedToTaskBoardTaskFormat = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat')
    .version('beta')
    .get();

```