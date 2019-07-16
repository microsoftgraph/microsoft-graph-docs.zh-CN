---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8fc3b65a3e2e92c0ee15c427194b6ef5863737dc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35737694"
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