---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 25072828b01ee4669bc02c3d2b39bc6f32e86b37
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartFont = {
  bold: true,
  color: "color-value",
  italic: true,
  name: "name-value",
  size: 99,
  underline: "underline-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .update({workbookChartFont : workbookChartFont});

```