---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 854528f9315a2cd8df2b907172eb8a1088abbeec
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123098"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2020-01-01T19:00:00-08:00"));
requestOptions.add(new QueryOption("endDateTime", "2020-01-02T19:00:00-08:00"));

IEventCollectionPage calendarView = graphClient.me().calendarView()
    .buildRequest( requestOptions )
    .get();

```