---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 890cf7e88d98a2103fc293297434dffaf6a357e4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: "Right",
  verticalAlignment: "Top",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format')
    .update(workbookRangeFormat);

```