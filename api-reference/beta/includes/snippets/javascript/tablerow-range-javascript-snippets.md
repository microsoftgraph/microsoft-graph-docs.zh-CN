---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 547e1a6daef16c4720e1ec0f72d2399d657bb2dd
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612813"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/Range')
    .version('beta')
    .post();

```