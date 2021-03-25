---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f7d22a3c4ea54ad9611c4cd40d5c47d2be5d3e9
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/chats/{chatId}";

String activityType = "taskCreated";

ItemBody previewText = new ItemBody();
previewText.content = "New Task Created";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "taskId";
templateParameters.value = "Task 12322";

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
        .withTeamsAppId(null)
        .build())
    .buildRequest()
    .post();

```