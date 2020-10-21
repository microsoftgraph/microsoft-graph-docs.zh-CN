---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd94bb2451548b0033e892bbfc2c382d10482fe7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606319"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3,
  values: [
    {
    }
  ]
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .post(workbookTableColumn);

```