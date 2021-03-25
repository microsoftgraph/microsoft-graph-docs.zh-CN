---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53b453169dd75703e300ab614680e797e102e0e3
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: 'PassthroughAuthentication rollout policy',
  description: 'PassthroughAuthentication rollout policy',
  feature: 'passthroughAuthentication',
  isEnabled: true,
  isAppliedToOrganization: false
};

await client.api('/policies/featureRolloutPolicies')
    .post(featureRolloutPolicy);

```