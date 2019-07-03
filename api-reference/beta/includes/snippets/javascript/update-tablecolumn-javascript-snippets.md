---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e878bd843278a13b7e695c8f73d13f1037c36e01
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479375"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  name: "name-value",
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .version('beta')
    .update({workbookTableColumn : workbookTableColumn});

```