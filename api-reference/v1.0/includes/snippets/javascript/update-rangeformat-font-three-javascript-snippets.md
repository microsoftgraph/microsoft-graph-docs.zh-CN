---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 716c9676abfff658a9f8ac9b3127dac34752b7ae
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: "Single",
  color: "#FFFFFF",
  size: 26
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$C$1')/format/font')
    .update({workbookRangeFont : workbookRangeFont});

```