---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 913c9dc893370ae4f0bd2090289fa9a03e03944c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35510013"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  id: 99,
  name: "name-value",
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .post({workbookTableColumn : workbookTableColumn});

```