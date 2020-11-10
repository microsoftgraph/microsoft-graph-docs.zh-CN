---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 003ab0c4090023bcf38d70e924308ab176b0d423
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954884"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "outlook.timezone=\"Pacific Standard Time\""));

Event event = graphClient.me().events("AAMkAGIAAAoZDOFAAA=")
    .buildRequest( requestOptions )
    .select("subject,body,bodyPreview,organizer,attendees,start,end,location")
    .get();

```