---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0bf3f69f12932f0d1d1e93786acd5a0d3536ddcc
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  values: "[
    [1, 2, 3],
    [4, 5, 6]
  ]"
};

await client.api('/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tables/Table1/rows')
    .version('beta')
    .post(workbookTableRow);

```