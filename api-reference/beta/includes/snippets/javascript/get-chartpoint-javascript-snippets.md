---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b16de44be74fa3ce537a20b3f93a7c3f1747aa5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48605100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/{undefined}')
    .version('beta')
    .get();

```