---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 760dc28af55c3322cad72929223341f6d80926a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucketTaskBoardTaskFormat = await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .get();

```