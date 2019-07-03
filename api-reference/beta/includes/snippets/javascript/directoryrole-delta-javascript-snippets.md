---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5636d2cd92bb4c0ca47707980ac348e3d8932f82
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499791"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```