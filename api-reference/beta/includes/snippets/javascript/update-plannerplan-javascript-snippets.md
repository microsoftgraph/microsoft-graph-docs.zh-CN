---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e677f1520064c45f4b6b6a18ccbde909b358ad97
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: "title-value"
};

let res = await client.api('/planner/plans/{id}')
    .version('beta')
    .update(plannerPlan);

```