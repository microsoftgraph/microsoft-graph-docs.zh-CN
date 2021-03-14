---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7fcdec3b23ff6c2a2fe6a9d7b3e1f14c8c78f15
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788689"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/directory/administrativeUnits/{id}')
    .delete();

```