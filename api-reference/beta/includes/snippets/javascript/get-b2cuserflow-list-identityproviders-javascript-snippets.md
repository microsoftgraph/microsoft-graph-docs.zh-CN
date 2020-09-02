---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 338562dcce8664ff7de4dbc41138f86b89d68703
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/{id}/identityProviders')
    .version('beta')
    .get();

```