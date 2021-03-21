---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08143cb00e31cb727d5c72e07a29ab9942fb58d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970519"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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