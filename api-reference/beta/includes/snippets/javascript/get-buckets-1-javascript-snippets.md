---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 438086a7eb25a2495e7bb50fda9d516c9ccf12e9e74656fd679c5fef23d4aa50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/buckets')
    .version('beta')
    .get();

```