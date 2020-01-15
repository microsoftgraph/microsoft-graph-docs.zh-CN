---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c729ee3016d6ec8cb986f536ad8e61c502facecf
ms.sourcegitcommit: 5f643d3b3f71a9711963c8953da2188539fc9b0c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/14/2020
ms.locfileid: "41123099"
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