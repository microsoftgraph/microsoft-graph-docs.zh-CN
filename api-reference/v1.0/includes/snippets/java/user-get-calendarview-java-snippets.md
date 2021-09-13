---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d1fa43975e7d33e1277f678b7338255fbe6066df3027dc56004a8c0d14c3d3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904079"
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