---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 271e5516b2f3b5bc431badaa4cfa86f29bd002cc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965151"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));
requestOptions.add(new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"));
requestOptions.add(new QueryOption("endDateTime", "2017-10-01T19:00:00.00-08:00"));

IEventCollectionPage calendarView = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").calendarView()
    .buildRequest( requestOptions )
    .get();

```