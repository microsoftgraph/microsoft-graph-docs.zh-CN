---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0b9e592a149737696c96c9902353709e963c3e2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971688"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Room place = new Room();
place.nickname = "Conf Room";
place.building = "1";
place.label = "100";
place.capacity = "50";
place.isWheelchairAccessible = false;

graphClient.places("cf100@contoso.com")
    .buildRequest()
    .patch(place);

```