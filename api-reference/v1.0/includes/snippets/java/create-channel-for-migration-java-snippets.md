---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19b24f1144255f9befafa76c8949df22a4979cf2
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508432"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Channel channel = new Channel();
channel.additionalDataManager().put("@microsoft.graph.channelCreationMode", new JsonPrimitive("migration"));
channel.displayName = "Import_150958_99z";
channel.description = "Import_150958_99z";
channel.createdDateTime = OffsetDateTimeSerializer.deserialize("2020-03-14T11:22:17.067Z");

graphClient.teams("57fb72d0-d811-46f4-8947-305e6072eaa5").channels()
    .buildRequest()
    .post(channel);

```