---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f85d6ba0aa1c506f47f0f6b91279a0e3ccb9b61e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603771"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .version('beta')
    .get();

```