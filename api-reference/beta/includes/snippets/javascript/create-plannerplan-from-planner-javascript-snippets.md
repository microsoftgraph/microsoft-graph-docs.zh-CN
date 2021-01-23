---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0df869ef2f3ed5245b6343d6c4e68d042c53515
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  container: {
    url: "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874"
  },
  title: "title-value"
};

let res = await client.api('/planner/plans')
    .version('beta')
    .post(plannerPlan);

```