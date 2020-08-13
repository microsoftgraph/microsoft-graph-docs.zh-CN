---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53af58f57786a9658deede2cf5bb79bf54058ce4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636621"
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

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/ItemAt')
    .version('beta')
    .post(workbookTableRow);

```