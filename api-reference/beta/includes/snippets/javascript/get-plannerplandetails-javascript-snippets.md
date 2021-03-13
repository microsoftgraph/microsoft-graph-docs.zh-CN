---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5121e3be560c156c7e70c6e58ecda8a78cadba26
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779594"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlanDetails = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .get();

```