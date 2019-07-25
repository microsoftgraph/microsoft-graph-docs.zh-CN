---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 26b96739f58e4e2eb99f93603e4fdf18c92d6194
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const _delete = {
  shift: "shift-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/delete')
    .version('beta')
    .post(_delete);

```