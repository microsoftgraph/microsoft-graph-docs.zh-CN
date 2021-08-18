---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df6ab97b2ad425f526412d9d84e4fd91e94706aaa77eb56760494c01b235f962
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.ENTITY_URL;
topic.value = "https://graph.microsoft.com/v1.0/users/{userId}/teamwork/installedApps/{installationId}";

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
        .build())
    .buildRequest()
    .post();

```