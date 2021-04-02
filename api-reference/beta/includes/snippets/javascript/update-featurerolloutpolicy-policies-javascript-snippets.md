---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20f3f1e3e6cf2281e8314a891617c41b8e698f69
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508601"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const featureRolloutPolicy = {
  displayName: 'PasswordHashSync Rollout Policy',
  description: 'PasswordHashSync Rollout Policy',
  isEnabled: true,
  isAppliedToOrganization: false
};

await client.api('/policies/featureRolloutPolicies/d7ab4886-d7f0-441b-a5e6-e62d7328d18a')
    .version('beta')
    .update(featureRolloutPolicy);

```