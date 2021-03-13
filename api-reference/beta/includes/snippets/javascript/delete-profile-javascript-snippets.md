---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ea3def8a3f7426a8443b4472293240f371cbe5bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795256"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile')
    .version('beta')
    .delete();

```