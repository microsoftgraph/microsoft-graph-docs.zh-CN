---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5366620ed60af2764626b63a9bed905585a0f8d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const device = {
  accountEnabled: false
};

await client.api('/devices/{id}')
    .version('beta')
    .update(device);

```