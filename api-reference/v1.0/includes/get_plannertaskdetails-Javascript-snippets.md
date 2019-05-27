---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 771ab96dbfa19856e1d8f5a9596c19873c47b576
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454678"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/details')
    .get();

```