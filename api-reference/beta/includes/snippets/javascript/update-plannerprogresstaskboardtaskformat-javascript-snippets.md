---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b0a54c3c46a8cb0d416445f0ffae2e7f035999c3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/{id}/progressTaskBoardFormat')
    .version('beta')
    .update(plannerProgressTaskBoardTaskFormat);

```