---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 077985459879a065e7df6d3dc05faec33d08a8a6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35728382"
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