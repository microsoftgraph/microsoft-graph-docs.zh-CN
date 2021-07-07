---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd44cb0d6adfef813c1c8530d35129908f21a1c6
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2021
ms.locfileid: "53317122"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/teams/e8bece96-d393-4b9b-b8da-69cedef1a7e7";

String activityType = "pendingFinanceApprovalRequests";

ItemBody previewText = new ItemBody();
previewText.content = "Internal spending team has a pending finance approval requests";

ChannelMembersNotificationRecipient recipient = new ChannelMembersNotificationRecipient();
recipient.teamId = "e8bece96-d393-4b9b-b8da-69cedef1a7e7";
recipient.channelId = "19:3d61a2309f094f4a9310b20f1db37520@thread.tacv2";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "pendingRequestCount";
templateParameters.value = "5";

templateParametersList.add(templateParameters);

graphClient.teams("e8bece96-d393-4b9b-b8da-69cedef1a7e7")
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