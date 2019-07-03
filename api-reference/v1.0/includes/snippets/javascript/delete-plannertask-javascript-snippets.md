---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f616a88b80b821d044975e669b40f7bc828adf14
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{id}')
    .delete();

```