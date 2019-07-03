---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 077985459879a065e7df6d3dc05faec33d08a8a6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}/summary')
    .version('beta')
    .get();

```