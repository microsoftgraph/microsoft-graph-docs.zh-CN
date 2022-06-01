---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3a034ffe9b1abc4f1704d3ec3b6b28cc4c9bfc8b
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819838"
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

LinkedList<TeamworkNotificationRecipient> recipientsList = new LinkedList<TeamworkNotificationRecipient>();
AadUserNotificationRecipient recipients = new AadUserNotificationRecipient();
recipients.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

recipientsList.add(recipients);
AadUserNotificationRecipient recipients1 = new AadUserNotificationRecipient();
recipients1.userId = "ab88234e-0874-477c-9638-d144296ed04f";

recipientsList.add(recipients1);
AadUserNotificationRecipient recipients2 = new AadUserNotificationRecipient();
recipients2.userId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc";

recipientsList.add(recipients2);

graphClient.teamwork()
    .sendActivityNotificationToRecipients(TeamworkSendActivityNotificationToRecipientsParameterSet
        .newBuilder()
        .withTopic(topic)
        .withActivityType(activityType)
        .withChainId(null)
        .withPreviewText(previewText)
        .withTeamsAppId(null)
        .withTemplateParameters(templateParametersList)
        .withRecipients(recipientsList)
        .build())
    .buildRequest()
    .post();

```