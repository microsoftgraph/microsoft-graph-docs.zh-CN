---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1e1fcad21170f0b5bdb35c81e72e7c3129857f38
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlan = await client.api('/planner/plans/{id}')
    .version('beta')
    .get();

```