---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03693acadebb12ede0047234e3cecd1e0b928a09
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/tables')
    .version('beta')
    .get();

```