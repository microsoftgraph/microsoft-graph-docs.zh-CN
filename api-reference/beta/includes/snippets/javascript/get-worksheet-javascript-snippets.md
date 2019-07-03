---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b99235181482a5e2f33e459d2df59dc11498ee3
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520994"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .version('beta')
    .get();

```