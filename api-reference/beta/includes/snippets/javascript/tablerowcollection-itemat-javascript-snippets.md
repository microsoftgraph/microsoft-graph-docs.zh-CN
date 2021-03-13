---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbdae00dc57b7926a39e6c7c7bfb0b1d907259c5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt')
    .version('beta')
    .post(workbookTableRow);

```