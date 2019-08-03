---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 032cb1c5f44255cfe3d1878e6c8371fda0e18b83
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172990"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/featureRolloutPolicies')
    .version('beta')
    .get();

```