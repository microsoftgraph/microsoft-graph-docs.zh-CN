---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69cfb8085e9d04582b2eaa0a7ce3d799998733db
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerProgressTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .get();

```