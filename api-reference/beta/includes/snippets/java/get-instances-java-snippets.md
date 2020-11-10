---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0592608b5d4544b7173f4ccb780d4aed6e54d35b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954815"
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