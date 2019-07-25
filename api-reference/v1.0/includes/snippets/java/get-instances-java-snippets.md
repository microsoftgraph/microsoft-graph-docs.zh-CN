---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0592608b5d4544b7173f4ccb780d4aed6e54d35b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35887306"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("startDateTime", "2019-04-08T09:00:00.0000000"));
requestOptions.add(new QueryOption("endDateTime", "2019-04-30T09:00:00.0000000"));

IEventCollectionPage instances = graphClient.me().events("AAMkAGUzYRgWAAA=").instances()
    .buildRequest( requestOptions )
    .select("subject,bodyPreview,seriesMasterId,type,recurrence,start,end")
    .get();

```