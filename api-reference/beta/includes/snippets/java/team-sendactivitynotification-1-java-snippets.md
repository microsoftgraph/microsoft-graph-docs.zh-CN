---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52e00af4ac7c0dcacc9968691701a20f596017d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954091"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/teams/{teamId}";

String activityType = "pendingFinanceApprovalRequests";

ItemBody previewText = new ItemBody();
previewText.content = "Internal spending team has a pending finance approval requests";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "pendingRequestCount";
templateParameters.value = "5";

templateParametersList.add(templateParameters);

graphClient.teams("{teamId}")
    .sendActivityNotification(topic,activityType,null,previewText,templateParametersList,recipient,null)
    .buildRequest()
    .post();

```