---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6cec0dbad2a5982d58f7d541e731f85089068d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795351"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  owner: 'ebf3b108-5234-4e22-b93d-656d7dae5874',
  title: 'title-value'
};

await client.api('/planner/plans')
    .post(plannerPlan);

```