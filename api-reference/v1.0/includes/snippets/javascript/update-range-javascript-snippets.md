---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05c1e870c39e4c64b50dfa15778571d9671c7439
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43770918"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
"values" : [["Hello", "100"],["1/1/2016", null]],
"formulas" : [[null, null], [null, "=B1*2"]],
"numberFormat" : [[null,null], ["m-ddd", null]]
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='A1:B2')')
    .update(workbookRange);

```