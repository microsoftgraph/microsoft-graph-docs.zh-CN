---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 385743327d5b2289d7846ba83cbd29cbf77ee71c
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48315454"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatMessage chatMessage = new ChatMessage();
ChatMessagePolicyViolation policyViolation = new ChatMessagePolicyViolation();
ChatMessagePolicyViolationPolicyTip policyTip = new ChatMessagePolicyViolationPolicyTip();
policyTip.generalText = "This item has been blocked by the administrator.";
policyTip.complianceUrl = "https://contoso.com/dlp-policy-page";
LinkedList<String> matchedConditionDescriptionsList = new LinkedList<String>();
matchedConditionDescriptionsList.add("Credit Card Number");
policyTip.matchedConditionDescriptions = matchedConditionDescriptionsList;
policyViolation.policyTip = policyTip;
policyViolation.verdictDetails = ChatMessagePolicyViolationVerdictDetailsTypes.ALLOW_OVERRIDE_WITHOUT_JUSTIFICATION;
policyViolation.dlpAction = ChatMessagePolicyViolationDlpActionTypes.BLOCK_ACCESS;
chatMessage.policyViolation = policyViolation;

graphClient.teams("e1234567-e123-4276-55555-6232b0e3a89a").channels("a7654321-e321-0000-0000-123b0e3a00a").messages("19:a21b0b0c05194ebc9e30000000000f61@thread.skype")
    .buildRequest()
    .patch(chatMessage);

```