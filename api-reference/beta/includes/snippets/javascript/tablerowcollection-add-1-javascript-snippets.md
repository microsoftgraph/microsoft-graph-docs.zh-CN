---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3885cf6d8fa4146e04a02fbaeaad71911b68fded
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952892"
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

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/add')
    .version('beta')
    .post(workbookTableRow);

```