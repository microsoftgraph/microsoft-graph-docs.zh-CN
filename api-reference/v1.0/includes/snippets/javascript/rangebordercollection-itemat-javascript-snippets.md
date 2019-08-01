---
description: 自动生成的文件。 不修改
ms.openlocfilehash: eddf334e15c58a42f961d03f4a7f94443ed13db3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeBorder = {
  index: 1
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/borders/itemAt')
    .post({workbookRangeBorder : workbookRangeBorder});

```