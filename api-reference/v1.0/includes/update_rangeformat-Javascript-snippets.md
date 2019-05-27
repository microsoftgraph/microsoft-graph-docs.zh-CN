---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aca4f3f5cefe804fa99d4f97f54b544030a28406
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  verticalAlignment: "Top",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$A$1')/format')
    .update({workbookRangeFormat : workbookRangeFormat});

```