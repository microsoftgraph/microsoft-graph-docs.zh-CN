---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd18c1c88ff5860d9e86dbbf5f990b8ccec84f46
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780413"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contract = await client.api('/contracts/{id}')
    .version('beta')
    .get();

```