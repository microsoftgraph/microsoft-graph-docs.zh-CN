---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8002daaefe7b65b589ee9bb08f2cabb1dc3f111b97dca42575b224e120804d60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54177835"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "odata.maxpagesize=2"));
requestOptions.add(new QueryOption("$skiptoken", "R0usmci39OQxqJrxK4"));

IEventDeltaCollectionPage delta = graphClient.me().calendarView()
    .delta()
    .buildRequest( requestOptions )
    .get();

```