---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbc2e6b2a42d6d4194eb4a456186d973686f4958
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787928"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 4
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt')
    .post(workbookTableRow);

```