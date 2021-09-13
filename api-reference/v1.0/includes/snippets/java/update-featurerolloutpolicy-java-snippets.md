---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 224e9fc790f3977b61f402a344f03cdf4b9682add612934b18ab6bdc6de791dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106438"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = new FeatureRolloutPolicy();
featureRolloutPolicy.displayName = "PasswordHashSync Rollout Policy";
featureRolloutPolicy.description = "PasswordHashSync Rollout Policy";
featureRolloutPolicy.isEnabled = true;
featureRolloutPolicy.isAppliedToOrganization = false;

graphClient.policies().featureRolloutPolicies("d7ab4886-d7f0-441b-a5e6-e62d7328d18a")
    .buildRequest()
    .patch(featureRolloutPolicy);

```