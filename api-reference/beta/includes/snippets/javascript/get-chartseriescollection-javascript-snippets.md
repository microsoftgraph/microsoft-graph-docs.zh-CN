---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fcc7255557ffd8d1ca7183c4c5f55be0a9b54363
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .version('beta')
    .get();

```