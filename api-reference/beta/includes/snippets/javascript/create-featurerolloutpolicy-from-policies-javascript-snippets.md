---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00a1ae04afc59d52a87510dc27ca562e8ed1bdeb0a5394ce8bb04815e1da5430
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221513"
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
    .version('beta')
    .post(featureRolloutPolicy);

```