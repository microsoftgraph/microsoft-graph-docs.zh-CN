---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9505222d638055aa4e4ec5fbc6c52a97afdecbd8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}')
    .get();

```