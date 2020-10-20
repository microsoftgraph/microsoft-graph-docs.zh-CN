---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 56834e164694d525d8d590b709921d9c5811fd75
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/format/fill/clear')
    .version('beta')
    .post();

```