---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 754b1a6e08a29d48f0b38b14f63d5c4ce10fed909120ae24c36cf24f6780bcb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  name: 'name-value',
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .update(workbookTableColumn);

```