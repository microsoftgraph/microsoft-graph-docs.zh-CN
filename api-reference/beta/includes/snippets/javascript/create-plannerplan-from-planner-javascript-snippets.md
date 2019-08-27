---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8c28808292b10be2b2506fdb0ac2fca3ce17989f
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  owner: "ebf3b108-5234-4e22-b93d-656d7dae5874",
  title: "title-value"
};

let res = await client.api('/planner/plans')
    .version('beta')
    .post(plannerPlan);

```