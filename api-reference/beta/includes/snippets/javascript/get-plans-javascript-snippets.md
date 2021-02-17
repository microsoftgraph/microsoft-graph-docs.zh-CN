---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bf0eed4eb4d4fd30de4e99ce7e31e96b2bf9622
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans')
    .version('beta')
    .get();

```