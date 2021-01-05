---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df4cb3b20f54c25e65e364fc76f6ef8e9a04ff19
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49754039"
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

LinkedList<KeyValuePair> templateParametersList = new LinkedList<KeyValuePair>();
KeyValuePair templateParameters = new KeyValuePair();
templateParameters.name = "deploymentId";
templateParameters.value = "6788662";

templateParametersList.add(templateParameters);

graphClient.users("{userId}").teamwork()
    .sendActivityNotification(topic,activityType,null,previewText,templateParametersList)
    .buildRequest()
    .post();

```