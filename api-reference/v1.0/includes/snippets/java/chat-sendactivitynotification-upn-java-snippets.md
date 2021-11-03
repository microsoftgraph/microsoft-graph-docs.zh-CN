---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 284cc06e2c891643df0435c915efe20856a5fa0a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696495"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}";

String activityType = "approvalRequired";

ItemBody previewText = new ItemBody();
previewText.content = "Deployment requires your approval";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "jacob@contoso.com";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "approvalTaskId";
templateParameters.value = "2020AAGGTAPP";

templateParametersList.add(templateParameters);

graphClient.chats("{chatId}")
    .sendActivityNotification(ChatSendActivityNotificationParameterSet
        .newBuilder()
        .withTopic(topic)
        .withActivityType(activityType)
        .withChainId(null)
        .withPreviewText(previewText)
        .withTemplateParameters(templateParametersList)
        .withRecipient(recipient)
        .build())
    .buildRequest()
    .post();

```