---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 593f3ed6b6b821dc48fd8bd60dbbab0f208fe9d0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/microsoft.graph.group')
    .get();

```