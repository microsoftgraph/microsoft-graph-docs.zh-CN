---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f73d58e3e4c2d0855224b4237ecdfddd317306fb
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945094"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  values: [
    [1, 2, 3],
    [4, 5, 6]
  ]
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/add')
    .version('beta')
    .post(workbookTableRow);

```