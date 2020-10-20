---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d89e31dd249b3c4b223eca25f9cccf1e56c11bdc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620822"
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
    .version('beta')
    .post(workbookNamedItem);

```