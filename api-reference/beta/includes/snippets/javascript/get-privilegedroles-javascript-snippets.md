---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 84b82dcb6546990bfc8753f81d28d7335cdeadce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles')
    .version('beta')
    .get();

```