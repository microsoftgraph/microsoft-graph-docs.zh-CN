---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a448b0d6ce1f21379c5eec975b1a13f63a56088
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753787"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.additionalDataManager().put("@microsoft.graph.channelCreationMode", new JsonPrimitive("migration"));
channel.displayName = "Architecture Discussion";
channel.description = "This channel is where we debate all future architecture plans";
channel.membershipType = ChannelMembershipType.STANDARD;
channel.createdDateTime = CalendarSerializer.deserialize("2020-03-14T11:22:17.067Z");

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels()
    .buildRequest()
    .post(channel);

```