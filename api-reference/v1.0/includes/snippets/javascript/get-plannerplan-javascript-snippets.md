---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c7e8c82f7bdee5c2a3b4e6686d1e1d9653ec9ba
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606202"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/{plan-id}')
    .get();

```