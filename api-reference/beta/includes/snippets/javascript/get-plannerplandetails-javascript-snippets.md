---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f03a2e09b5285b55ac3de6a3e3ce8cf7069bbd20
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730358"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .get();

```