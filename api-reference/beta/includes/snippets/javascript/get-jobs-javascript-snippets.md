---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d00d7b88b968bd642d9b1a48bc5d164c550f405f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35717399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/')
    .version('beta')
    .get();

```