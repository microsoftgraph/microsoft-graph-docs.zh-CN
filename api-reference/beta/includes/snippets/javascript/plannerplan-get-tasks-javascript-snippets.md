---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5d9d95f64564e395e5c269ff77c5761e7587b99
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789948"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/tasks')
    .version('beta')
    .get();

```