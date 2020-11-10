---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0022a5c50b1a284186bc9478f72a03d2c4cacc3d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957918"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConditionalAccessPolicy conditionalAccessPolicy = new ConditionalAccessPolicy();
ConditionalAccessConditionSet conditions = new ConditionalAccessConditionSet();
LinkedList<RiskLevel> signInRiskLevelsList = new LinkedList<RiskLevel>();
signInRiskLevelsList.add(RiskLevel.HIGH);
signInRiskLevelsList.add(RiskLevel.MEDIUM);
signInRiskLevelsList.add(RiskLevel.LOW);
conditions.signInRiskLevels = signInRiskLevelsList;
conditionalAccessPolicy.conditions = conditions;

graphClient.identity().conditionalAccess().policies("{id}")
    .buildRequest()
    .patch(conditionalAccessPolicy);

```