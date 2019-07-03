---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c0abad1f53cd3962ce4fb12d14f7d3d0f713796c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521553"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/resources/{id}/content')
    .version('beta')
    .get();

```