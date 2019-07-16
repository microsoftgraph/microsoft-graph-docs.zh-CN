---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 662175dc3dec94c6548d6a4051420e19676a11d0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736801"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/usedRange(valuesOnly=true)')
    .get();

```