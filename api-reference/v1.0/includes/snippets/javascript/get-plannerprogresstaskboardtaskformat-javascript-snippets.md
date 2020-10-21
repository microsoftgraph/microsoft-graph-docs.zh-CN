---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fde94a6613d39fc44b51fd9775132d86b267282
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48616145"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .get();

```