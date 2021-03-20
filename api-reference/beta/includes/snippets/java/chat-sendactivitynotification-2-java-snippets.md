---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 566f2e8c0026f36daade8c0a3f97872765a732bb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948005"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}";

String activityType = "approvalRequired";

ItemBody previewText = new ItemBody();
previewText.content = "Deployment requires your approval";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "approvalTaskId";
templateParameters.value = "2020AAGGTAPP";

templateParametersList.add(templateParameters);

graphClient.chats("{chatId}")
    .sendActivityNotification(topic,activityType,null,previewText,templateParametersList,recipient,null)
    .buildRequest()
    .post();

```