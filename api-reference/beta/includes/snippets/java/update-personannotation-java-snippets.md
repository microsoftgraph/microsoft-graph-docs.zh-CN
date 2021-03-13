---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7bf1f486edd38ee7aa9510e5dbc2fc0c7d418784
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774171"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = new PersonAnnotation();
personAnnotation.allowedAudiences = EnumSet.of(AllowedAudiences.ORGANIZATION);

graphClient.users("{userId}").profile().notes("{id}")
    .buildRequest()
    .patch(personAnnotation);

```