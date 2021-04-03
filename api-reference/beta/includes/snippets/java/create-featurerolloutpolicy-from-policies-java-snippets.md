---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6db16241a5aa507ae850890047d7d9521a28154
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

FeatureRolloutPolicy featureRolloutPolicy = new FeatureRolloutPolicy();
featureRolloutPolicy.displayName = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.description = "PassthroughAuthentication rollout policy";
featureRolloutPolicy.feature = StagedFeatureName.PASSTHROUGH_AUTHENTICATION;
featureRolloutPolicy.isEnabled = true;
featureRolloutPolicy.isAppliedToOrganization = false;

graphClient.policies().featureRolloutPolicies()
    .buildRequest()
    .post(featureRolloutPolicy);

```