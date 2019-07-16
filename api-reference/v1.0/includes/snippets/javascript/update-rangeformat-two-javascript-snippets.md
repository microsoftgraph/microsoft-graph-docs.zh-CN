---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 706f7c9d23600fc937776dc88266d10693fedc99
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: "Center",
  verticalAlignment: "Center",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format')
    .update({workbookRangeFormat : workbookRangeFormat});

```