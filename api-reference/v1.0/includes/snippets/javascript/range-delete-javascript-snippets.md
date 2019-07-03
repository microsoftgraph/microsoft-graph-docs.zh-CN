---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 67c89aaf68e7dcda76e5f30837b3913808004c9d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509865"
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
    .post(_delete);

```