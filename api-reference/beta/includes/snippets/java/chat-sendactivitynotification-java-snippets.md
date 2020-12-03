---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fea283399cbbf1b370778b0fbcb25c759b4ec04a
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521976"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkActivityTopic topic = new TeamworkActivityTopic();
topic.source = TeamworkActivityTopicSource.TEXT;
topic.value = "Deployment Approvals Channel";
topic.webUrl = "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000";

String activityType = "deploymentApprovalRequired";

ItemBody previewText = new ItemBody();
previewText.content = "New deployment requires your approval";

AadUserNotificationRecipient recipient = new AadUserNotificationRecipient();
recipient.userId = "569363e2-4e49-4661-87f2-16f245c5d66a";

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "deploymentId";
templateParameters.value = "6788662";

templateParametersList.add(templateParameters);

graphClient.chats("{chatId}")
    .sendActivityNotification(topic,activityType,null,previewText,templateParametersList,recipient)
    .buildRequest()
    .post();

```