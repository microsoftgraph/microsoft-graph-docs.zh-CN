---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8fc3b65a3e2e92c0ee15c427194b6ef5863737dc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493368"
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
    .post(unprotect);

```