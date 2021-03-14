---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af08754964cddf1213e4cb731c871836faf5e3d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let notebooks = await client.api('/me/onenote/notebooks')
    .get();

```