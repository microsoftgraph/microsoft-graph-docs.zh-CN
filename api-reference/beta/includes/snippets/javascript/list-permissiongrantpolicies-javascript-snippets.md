---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ab22556e67639fbcf5cd99c81ede4e5b977e37a
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/permissionGrantPolicies')
    .version('beta')
    .get();

```