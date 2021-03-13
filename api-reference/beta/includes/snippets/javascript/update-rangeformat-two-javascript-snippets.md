---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1da87fd54e1f5ea9cd4c5f02a2d1fe0278fd6076
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782590"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: 'Center',
  verticalAlignment: 'Center',
  rowHeight: 49,
  wrapText: false
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format')
    .version('beta')
    .update(workbookRangeFormat);

```