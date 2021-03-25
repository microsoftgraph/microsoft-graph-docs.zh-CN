---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 378278b1ee92cb805ad2b39c44856abfd3910299
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211076"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/teams/{teamId}/channels/{channelId}/tabs/{tabId}";

String activityType = "reservationUpdated";

ItemBody previewText = new ItemBody();
previewText.content = "You have moved up the queue";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

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
        .withTeamsAppId(null)
        .build())
    .buildRequest()
    .post();

```