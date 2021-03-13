---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4cce694ec2d31d2373dcd189d2b3a6e1cfd47ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771475"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/groups/{groupId}"));

graphClient.print().shares("{printerShareId}").allowedGroups().references()
    .buildRequest()
    .post(group);

```