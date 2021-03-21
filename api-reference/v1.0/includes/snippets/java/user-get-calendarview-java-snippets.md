---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33a8db40ae68dd1c4ea6ee1bfdffc8dcea2cc9d3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980359"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2020-01-01T19:00:00-08:00"));
requestOptions.add(new QueryOption("endDateTime", "2020-01-02T19:00:00-08:00"));

EventCollectionPage calendarView = graphClient.me().calendarView()
    .buildRequest( requestOptions )
    .get();

```