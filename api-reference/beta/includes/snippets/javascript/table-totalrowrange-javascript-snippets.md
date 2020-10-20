---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e822f3d2dde6dc4ebc6abcb7356de75c7d94032f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/TotalRowRange')
    .version('beta')
    .post();

```