---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2e78f4f9220874dde075423c4bf004aef3e30aa
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id|userPrincipalName}/manager')
    .version('beta')
    .get();

```