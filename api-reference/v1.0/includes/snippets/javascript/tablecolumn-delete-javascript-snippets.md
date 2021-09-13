---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b071e9866b5f7eb3531125350d8b9086b74bb6bf98de7060cbb016ddde04947
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}')
    .delete();

```