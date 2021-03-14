---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ceb2f7258cbeceafbc51b11f8151ed6e35ecc06d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779517"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .update(plannerProgressTaskBoardTaskFormat);

```