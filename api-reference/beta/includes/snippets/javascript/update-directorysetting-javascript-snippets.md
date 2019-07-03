---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 2a02ac999b23ffce68347a1d1823af8ba81de32d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directorySetting = {
  values: [
    {
      name: "name-value",
      value: "value-value"
    }
  ]
};

let res = await client.api('/settings/{id}')
    .version('beta')
    .update({directorySetting : directorySetting});

```