---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3943809558019e4ac87be1fb67905bf420889c5
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60691587"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/v1.0/teams/{teamId}/channels/{channelId}/tabs/{tabId}";

String activityType = "reservationUpdated";

ItemBody previewText = new ItemBody();
previewText.content = "You have moved up the queue";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "jacob@contoso.com";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "reservationId";
templateParameters.value = "TREEE433";

templateParametersList.add(templateParameters);
KeyValuePair templateParameters1 = new KeyValuePair();
templateParameters1.name = "currentSlot";
templateParameters1.value = "23";

templateParametersList.add(templateParameters1);

graphClient.teams("{teamId}")
    .sendActivityNotification(TeamSendActivityNotificationParameterSet
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