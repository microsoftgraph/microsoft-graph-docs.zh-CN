---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c8c326c1e7bb7d83680fbe4ef2568b205deb8551
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733269"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}/buckets')
    .get();

```