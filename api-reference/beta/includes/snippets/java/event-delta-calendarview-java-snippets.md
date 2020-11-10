---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e06d179194324f38b94e6029b85801fe51ac29a7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954856"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2020-06-01T00:00:00Z"));
requestOptions.add(new QueryOption("endDateTime", "2020-06-10T00:00:00Z"));

IEventDeltaCollectionPage delta = graphClient.me().calendars("AAMkADI5M1BbeAAA=").calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```