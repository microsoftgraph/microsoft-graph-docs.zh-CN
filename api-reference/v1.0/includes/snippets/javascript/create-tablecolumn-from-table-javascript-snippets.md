---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e948def7328b600e7652a5b21162142b3074a325c618903aeb4b7bb5c7c92e1d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219992"
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