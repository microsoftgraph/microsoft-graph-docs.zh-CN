---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1c7e8c82f7bdee5c2a3b4e6686d1e1d9653ec9ba
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}')
    .get();

```