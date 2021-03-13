---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fc03e53d9730bad9558bf3dc275eae140881566
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRange = {
values: [['Hello', '100'],['1/1/2016', null]],
formulas: [[null, null], [null, '=B1*2']],
numberFormat: [[null,null], ['m-ddd', null]]
};

await client.api('/me/drive/items/{id}/workbook/worksheets/sheet1/range(address='A1:B2')')
    .version('beta')
    .update(workbookRange);

```