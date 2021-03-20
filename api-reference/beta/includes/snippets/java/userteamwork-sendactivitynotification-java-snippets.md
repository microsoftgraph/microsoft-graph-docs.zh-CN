---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7509920b052e979ce7ada7ed1e1b450c507ab13
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941933"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/beta/users/{userId}/teamwork/installedApps/{installationId}";

String activityType = "taskCreated";

ItemBody previewText = new ItemBody();
previewText.content = "New Task Created";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "taskId";
templateParameters.value = "Task 12322";

templateParametersList.add(templateParameters);

graphClient.users("{userId}").teamwork()
    .sendActivityNotification(UserTeamworkSendActivityNotificationParameterSet
        .newBuilder()
        .withTopic(topic)
        .withActivityType(activityType)
        .withChainId(null)
        .withPreviewText(previewText)
        .withTemplateParameters(templateParametersList)
        .withTeamsAppId(null)
        .build())
    .buildRequest()
    .post();

```