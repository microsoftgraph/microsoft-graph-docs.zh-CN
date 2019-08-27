---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ee825afa353e0edbc274e0d6024694656503afd7
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636538"
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
    .post(featureRolloutPolicy);

```