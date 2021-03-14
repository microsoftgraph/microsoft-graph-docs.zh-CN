---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0638f6a2097b7a9a5992e83ffa556f2f1030997d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: 'applyTo-value'
};

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .post(clear);

```