---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5ddcb128b6114fdaaac37fc7a89dd255909ff74e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh')
    .version('beta')
    .get();

```