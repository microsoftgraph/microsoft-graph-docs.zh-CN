---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71341c16759af11a27e5510b7085405f37c25ac2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookWorksheet = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .version('beta')
    .get();

```