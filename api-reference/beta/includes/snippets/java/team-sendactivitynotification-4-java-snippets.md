---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f3af2ecf03493933282ca006dea45351384a60
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.TEXT;
topic.value = "Deployment Approvals Channel";
topic.webUrl = "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000";

String activityType = "deploymentApprovalRequired";

ItemBody previewText = new ItemBody();
previewText.content = "New deployment requires your approval";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "deploymentId";
templateParameters.value = "6788662";

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