---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5b8b3119070a59a56ca0624a82f63f27b240a673fdb2beb2675cc8cf49a16df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221115"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.body-content-type=\"text\""));
requestOptions.add(new QueryOption("startDateTime", "2017-01-01T19:00:00-08:00"));
requestOptions.add(new QueryOption("endDateTime", "2017-10-01T19:00:00.00-08:00"));

EventCollectionPage calendarView = graphClient.groups("02bd9fd6-8f93-4758-87c3-1fb73740a315").calendarView()
    .buildRequest( requestOptions )
    .get();

```