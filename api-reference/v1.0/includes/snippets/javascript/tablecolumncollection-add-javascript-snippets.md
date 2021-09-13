---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca2261095ececdd9e0f08a53ef2a4e6a3c1ba2499278149896e188c10a8e0e55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273832"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3,
  values: [
    {
    }
  ]
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/add')
    .post(workbookTableColumn);

```