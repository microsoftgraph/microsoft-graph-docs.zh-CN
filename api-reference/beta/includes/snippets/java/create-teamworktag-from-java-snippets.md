---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6280a63ea202b4cf214b25a16196af875d79c6d0
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamworkTag teamworkTag = new TeamworkTag();
teamworkTag.displayName = "Finance";
LinkedList<TeamworkTagMember> membersList = new LinkedList<TeamworkTagMember>();
TeamworkTagMember members = new TeamworkTagMember();
members.userId = "92f6952f-61ca-4a94-8910-508a240bc167";
membersList.add(members);
TeamworkTagMember members1 = new TeamworkTagMember();
members1.userId = "085d800c-b86b-4bfc-a857-9371ad1caf29";
membersList.add(members1);
TeamworkTagMemberCollectionResponse teamworkTagMemberCollectionResponse = new TeamworkTagMemberCollectionResponse();
teamworkTagMemberCollectionResponse.value = membersList;
TeamworkTagMemberCollectionPage teamworkTagMemberCollectionPage = new TeamworkTagMemberCollectionPage(teamworkTagMemberCollectionResponse, null);
teamworkTag.members = teamworkTagMemberCollectionPage;

graphClient.teams("53c53217-fe77-4383-bc5a-ed4937a1aecd").tags()
    .buildRequest()
    .post(teamworkTag);

```