---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c043b4f335343d3e0c19a2025d75838ec41dfabd
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48984195"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("members@odata.bind", new JsonPrimitive("[  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\",  \"https://graph.microsoft.com/v1.0/directoryObjects/{id}\"]"));

graphClient.groups("{group-id}")
    .buildRequest()
    .patch(group);

```