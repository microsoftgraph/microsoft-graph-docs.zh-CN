---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aeac5e9a69609ea8e414d7529d1ca9e64e6c3570
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFont = {
  underline: 'Single',
  color: '#FFFFFF',
  size: 26
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/font')
    .version('beta')
    .update(workbookRangeFont);

```