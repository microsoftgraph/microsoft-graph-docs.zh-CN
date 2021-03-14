---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00ea6f6cb9f01181852905a769142fdd37d8fe6e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  italic: true,
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{sheet-id}/range(address='$B$1')/format/font')
    .update(workbookRangeFont);

```