---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7a8668bd5635d92b9f2077eff4488e22b6de3829
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35858501"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));
requestOptions.add(new QueryOption("startDateTime", "2017-01-01T19:00:00.0000000"));
requestOptions.add(new QueryOption("endDateTime", "2017-10-01T19:00:00.00"));

IEventCollectionPage calendarView = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").calendarView()
    .buildRequest( requestOptions )
    .get();

```