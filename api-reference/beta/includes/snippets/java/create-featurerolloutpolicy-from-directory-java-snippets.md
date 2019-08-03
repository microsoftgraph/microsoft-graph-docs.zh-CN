---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 391b7034589233300f6f1794c8c6b6fe286f697a
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36172952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = new FeatureRolloutPolicy();
featureRolloutPolicy.displayName = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.description = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.feature = StagedFeatureName.PASSTHROUGH_AUTHENTICATION;
featureRolloutPolicy.isEnabled = true;
featureRolloutPolicy.isAppliedToOrganization = false;

graphClient.directory().featureRolloutPolicies()
    .buildRequest()
    .post(featureRolloutPolicy);

```