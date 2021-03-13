---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b672f514ca283e8d1c37fd5cc5c678b7aa846c78
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: '#FF0000'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format/fill')
    .version('beta')
    .update(workbookRangeFill);

```