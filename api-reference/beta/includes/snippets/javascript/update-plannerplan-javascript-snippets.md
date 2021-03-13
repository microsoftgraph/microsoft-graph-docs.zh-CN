---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c66240b828f80cf814bbf65df6ea7fc34397463b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805408"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: 'title-value'
};

await client.api('/planner/plans/{id}')
    .version('beta')
    .update(plannerPlan);

```