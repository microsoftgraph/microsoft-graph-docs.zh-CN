---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4175fa615439b233e15262e61ef017c1cafbaa0f2cb67391b2feade418c8ddfd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177830"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));
requestOptions.add(new QueryOption("startdatetime", "2016-12-01T00:00:00Z"));
requestOptions.add(new QueryOption("enddatetime", "2016-12-30T00:00:00Z"));

IEventDeltaCollectionPage delta = graphClient.me().calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```