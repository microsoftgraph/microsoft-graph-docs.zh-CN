---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66da367292f9a2ddbb826e94e7f1f6753286cdae
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974727"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonAnnotation personAnnotation = new PersonAnnotation();
ItemBody detail = new ItemBody();
detail.contentType = BodyType.TEXT;
detail.content = "I am originally from Australia, but grew up in Moscow, Russia.";
personAnnotation.detail = detail;
personAnnotation.displayName = "About Me";

graphClient.me().profile().notes()
    .buildRequest()
    .post(personAnnotation);

```