---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c1196cf79ecf7260b9829efa5a6632d004f5bce1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727764"
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

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')')
    .version('beta')
    .update(workbookRange);

```