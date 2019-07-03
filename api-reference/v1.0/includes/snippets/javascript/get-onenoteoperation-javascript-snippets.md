---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 79c9a7ea97011b26f0dde23a02a8e99a8a730860
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35509311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/operations/{id}')
    .get();

```