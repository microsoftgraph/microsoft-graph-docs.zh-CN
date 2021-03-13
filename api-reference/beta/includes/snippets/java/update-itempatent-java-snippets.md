---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 716f2a2be9fef5cbfef310691ceb5dfb4164881c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777788"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPatent itemPatent = new ItemPatent();
itemPatent.number = "USPTO-3954432633";
itemPatent.webUrl = "https://patents.gov/3954432633";

graphClient.users("{userId}").profile().patents("{id}")
    .buildRequest()
    .patch(itemPatent);

```