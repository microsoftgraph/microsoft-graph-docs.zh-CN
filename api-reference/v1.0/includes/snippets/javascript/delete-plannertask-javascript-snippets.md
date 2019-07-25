---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f616a88b80b821d044975e669b40f7bc828adf14
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{id}')
    .delete();

```