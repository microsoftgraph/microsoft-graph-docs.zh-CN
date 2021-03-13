---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 341f38b18bd57211b3312214ca9392eb4f206a82
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798035"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: 'Right',
  verticalAlignment: 'Top',
  rowHeight: 49,
  wrapText: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format')
    .version('beta')
    .update(workbookRangeFormat);

```