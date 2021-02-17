---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38d446439426c93d00ef06b2149ef8e8d6ec0efa
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{usersId}/planner/rosterPlans')
    .version('beta')
    .get();

```