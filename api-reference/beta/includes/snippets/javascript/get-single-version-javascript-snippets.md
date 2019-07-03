---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 55ae26fb4f3dcf1d16bb55d8a8ca84fadb5f23f6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521142"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .version('beta')
    .get();

```