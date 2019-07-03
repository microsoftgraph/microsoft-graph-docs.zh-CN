---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6f3018c42baf076f064861b43f03d62744be5e9b
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookNamedItem = {
  name: "test7",
  formula: "=SUM(Sheet2!$A$1+Sheet2!$A$2)",
  comment: "Comment for the named item"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/addFormulaLocal')
    .post(workbookNamedItem);

```