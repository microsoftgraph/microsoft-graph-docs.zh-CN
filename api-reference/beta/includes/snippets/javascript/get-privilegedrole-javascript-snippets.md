---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f4fc40343f031dfbdf5f0b2712b6e3f496a7684f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796939"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRole = await client.api('/privilegedRoles/{id}')
    .version('beta')
    .get();

```