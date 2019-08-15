---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e8f8757e1d48132b1dae65900c438986ebcc831
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{id}/progressTaskBoardFormat')
    .version('beta')
    .get();

```