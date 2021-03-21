---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cae81a63c5d7477224e6332efa99bdb5de00115
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954095"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
    .sendActivityNotification(topic,activityType,null,previewText,templateParametersList,recipient,null)
    .buildRequest()
    .post();

```