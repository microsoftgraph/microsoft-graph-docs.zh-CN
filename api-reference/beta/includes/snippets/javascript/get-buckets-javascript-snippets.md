---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b171198595dd9eb271f90167b2ed6f660c9a598b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/2txjA-BMZEq-bKi6Wfj5aGQAB1OJ/buckets')
    .version('beta')
    .get();

```