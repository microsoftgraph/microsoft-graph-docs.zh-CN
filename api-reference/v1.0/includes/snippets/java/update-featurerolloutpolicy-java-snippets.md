---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3eaf391017d2d12115230020835ce0db70cc513
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201260"
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