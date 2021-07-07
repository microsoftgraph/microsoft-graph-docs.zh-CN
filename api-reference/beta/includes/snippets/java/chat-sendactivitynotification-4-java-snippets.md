---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2ae7e5cbb97f203f04f2e40d40fd6a0ac50b3cc
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/chats/19:1c3af46e9e0f4a5293343c8813c47619@thread.v2";

String activityType = "taskCreated";

ItemBody previewText = new ItemBody();
previewText.content = "New Task Created";

ChatMembersNotificationRecipient recipient = new ChatMembersNotificationRecipient();
recipient.chatId = "19:1c3af46e9e0f4a5293343c8813c47619@thread.v2";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "taskId";
templateParameters.value = "Task 12322";

templateParametersList.add(templateParameters);

graphClient.chats("19:1c3af46e9e0f4a5293343c8813c47619@thread.v2")
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