---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c7de362b5188b04ee7584ccddccec61f933c3a6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unprotect = {
  password: "password-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .version('beta')
    .post(unprotect);

```