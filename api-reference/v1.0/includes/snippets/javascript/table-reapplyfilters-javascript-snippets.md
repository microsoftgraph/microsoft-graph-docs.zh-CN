---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 632ed65793b20a13ba5055337cdf5d59a5b2bd58
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters')
    .post();

```