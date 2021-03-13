---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1840d5cf7d82fa17acd2916e365f4ee2e3984cd0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```