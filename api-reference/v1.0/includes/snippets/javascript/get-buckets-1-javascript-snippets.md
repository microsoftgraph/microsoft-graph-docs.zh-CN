---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0d744d11440932827a139f4528055bad43d5ac90d01c24e344cb815d0333c47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/buckets')
    .get();

```