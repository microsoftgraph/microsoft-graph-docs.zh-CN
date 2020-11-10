---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c729ee3016d6ec8cb986f536ad8e61c502facecf
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960047"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"));
requestOptions.add(new QueryOption("endDateTime", "2017-01-07T19:00:00-08:00"));

IEventCollectionPage calendarView = graphClient.me().calendar().calendarView()
    .buildRequest( requestOptions )
    .get();

```