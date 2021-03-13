---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ea2275e1c86f07cd207d894df089d1b828cfd22
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797041"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  container: {
    url: 'https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874'
  },
  title: 'title-value'
};

await client.api('/planner/plans')
    .version('beta')
    .post(plannerPlan);

```