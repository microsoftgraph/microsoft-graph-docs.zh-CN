---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 398f3d28b42378ee3eb3f596a05a3fc791b81058
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let permissions = await client.api('/me/drive/items/{item-id}/permissions')
    .version('beta')
    .get();

```