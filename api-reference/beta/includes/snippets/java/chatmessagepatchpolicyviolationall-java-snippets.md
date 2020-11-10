---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b851a86a5cf4322f20a599bebd891b0db50b2a80
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48958114"
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
policyViolation.verdictDetails = EnumSet.of(ChatMessagePolicyViolationVerdictDetailsTypes.ALLOW_OVERRIDE_WITHOUT_JUSTIFICATION,ChatMessagePolicyViolationVerdictDetailsTypes.ALLOW_FALSE_POSITIVE_OVERRIDE);
policyViolation.dlpAction = EnumSet.of(ChatMessagePolicyViolationDlpActionTypes.BLOCK_ACCESS);
chatMessage.policyViolation = policyViolation;

graphClient.teams("e1234567-e123-4276-55555-6232b0e3a89a").channels("a7654321-e321-0000-0000-123b0e3a00a").messages("19:a21b0b0c05194ebc9e30000000000f61@thread.skype")
    .buildRequest()
    .patch(chatMessage);

```