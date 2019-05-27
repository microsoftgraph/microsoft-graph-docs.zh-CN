---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1f609ff13f09d799c5f1baad3103f18133f7111c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  bold: true,
  color: "color-value",
  italic: true,
  name: "name-value",
  size: 99,
  underline: "underline-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/font')
    .version('beta')
    .update({workbookRangeFont : workbookRangeFont});

```