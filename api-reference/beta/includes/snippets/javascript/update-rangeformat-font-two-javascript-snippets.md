---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 382feb51cd8778e6e3c43e0e71f40939b9b62472
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636649"
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

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$B$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```