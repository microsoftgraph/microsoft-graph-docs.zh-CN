---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e7dc9a684cfa43f11008f6151ac0e9c773904e94
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "A1:D8",
  hasHeaders: false
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/$/add')
    .version('beta')
    .post(workbookTable);

```