---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a22b60b93194f5bec47214639ec772a469905d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let featureRolloutPolicies = await client.api('/directory/featureRolloutPolicies')
    .version('beta')
    .get();

```