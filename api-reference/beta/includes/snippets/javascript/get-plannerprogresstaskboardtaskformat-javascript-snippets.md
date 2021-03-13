---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98adf50e28d4b840bb21a67e51941b1f342c60c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802404"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerProgressTaskBoardTaskFormat = await client.api('/planner/tasks/{id}/progressTaskBoardFormat')
    .version('beta')
    .get();

```