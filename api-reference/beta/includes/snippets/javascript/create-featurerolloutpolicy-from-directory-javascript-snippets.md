---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1501dfe7860e11b18eebf2c712caef7dbc25da90
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: "PassthroughAuthentication rollout policy",
  description: "PassthroughAuthentication rollout policy",
  feature: "passthroughAuthentication",
  isEnabled: true,
  isAppliedToOrganization: false
};

let res = await client.api('/directory/featureRolloutPolicies')
    .version('beta')
    .post({featureRolloutPolicy : featureRolloutPolicy});

```