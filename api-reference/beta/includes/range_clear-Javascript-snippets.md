---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b3f9728e237800e3ea2617952e3e7c469765ad76
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const clear = {
  applyTo: "applyTo-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/clear')
    .version('beta')
    .post(clear);

```