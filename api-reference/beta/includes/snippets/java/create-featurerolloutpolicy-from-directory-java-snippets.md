---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 391b7034589233300f6f1794c8c6b6fe286f697a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48963216"
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