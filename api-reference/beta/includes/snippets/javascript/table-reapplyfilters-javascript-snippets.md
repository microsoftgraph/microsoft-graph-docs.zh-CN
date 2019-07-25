---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a9f557f94a255178c118da5ef1a26f722c96939
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters')
    .version('beta')
    .post();

```