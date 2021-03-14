---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c7d0bf7bce2c5b71fd712decd9f311ff4fd4c37
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableColumn = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .get();

```