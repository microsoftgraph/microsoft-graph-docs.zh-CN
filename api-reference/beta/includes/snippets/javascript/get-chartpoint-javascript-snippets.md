---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9b16de44be74fa3ce537a20b3f93a7c3f1747aa5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463644"
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