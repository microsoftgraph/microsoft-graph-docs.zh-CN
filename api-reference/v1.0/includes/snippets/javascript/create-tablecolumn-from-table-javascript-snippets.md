---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31fa2b6808b83704f39c04ce04bf858ddde3689c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  id: '99',
  name: 'name-value',
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .post(workbookTableColumn);

```