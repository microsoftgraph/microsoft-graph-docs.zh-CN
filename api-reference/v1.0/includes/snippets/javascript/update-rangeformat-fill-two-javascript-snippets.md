---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 760cdc66fcd57338feaca3d8ca1511225645c721
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493211"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#00FF00"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```