---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 69e039f9bb212373db571577c6f63cd9c6a8b129
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .update({plannerProgressTaskBoardTaskFormat : plannerProgressTaskBoardTaskFormat});

```