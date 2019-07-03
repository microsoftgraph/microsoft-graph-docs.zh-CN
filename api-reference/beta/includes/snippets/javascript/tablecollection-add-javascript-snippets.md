---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99a4d2260adb897c8732a4d48a32021ed0e206cd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478565"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "Sheet1!A1:D5",
  hasHeaders: true
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/add')
    .version('beta')
    .post(workbookTable);

```