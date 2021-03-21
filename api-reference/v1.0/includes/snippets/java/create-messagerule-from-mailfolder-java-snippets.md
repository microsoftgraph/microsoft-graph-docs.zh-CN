---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc72981807fa78c2e1d1d9c93e86cf41087aed14
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979449"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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