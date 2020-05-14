---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1871c37dfb8656fa587ab68de9c135acc2cb052
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35856393"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

MessageRule messageRule = new MessageRule();
messageRule.displayName = "From partner";
messageRule.sequence = 2;
messageRule.isEnabled = true;
MessageRulePredicates conditions = new MessageRulePredicates();
LinkedList<String> senderContainsList = new LinkedList<String>();
senderContainsList.add("adele");
conditions.senderContains = senderContainsList;
messageRule.conditions = conditions;
MessageRuleActions actions = new MessageRuleActions();
LinkedList<Recipient> forwardToList = new LinkedList<Recipient>();
Recipient forwardTo = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "Alex Wilbur";
emailAddress.address = "AlexW@contoso.onmicrosoft.com";
forwardTo.emailAddress = emailAddress;
forwardToList.add(forwardTo);
actions.forwardTo = forwardToList;
actions.stopProcessingRules = true;
messageRule.actions = actions;

graphClient.me().mailFolders("inbox").messageRules()
    .buildRequest()
    .post(messageRule);

```