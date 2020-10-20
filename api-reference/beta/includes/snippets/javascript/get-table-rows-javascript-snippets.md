---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cddbe34e9d477a846a934f828882d0af125e8e3
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .skip(5)
    .top(5)
    .get();

```