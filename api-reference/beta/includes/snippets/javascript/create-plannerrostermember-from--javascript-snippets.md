---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 834eecaade10b7f85b9214d126153d66ccdadb63
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRosterMember = {
  @odata.type: "#microsoft.graph.plannerRosterMember",
  userId: "String"
};

let res = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965/members')
    .version('beta')
    .post(plannerRosterMember);

```