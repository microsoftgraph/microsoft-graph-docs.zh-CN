---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a573b42a3e9845a8480a8bfd9921e9f9ed00d3617a8772e4eb1bd673d2594574
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221299"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rosterPlans = await client.api('/users/{usersId}/planner/rosterPlans')
    .version('beta')
    .get();

```