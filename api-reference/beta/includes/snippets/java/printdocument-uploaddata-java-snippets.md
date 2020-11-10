---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f264f700646dea984c1fc2b86833e24279691160
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980977"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Range", "bytes=0-72796"));

graphClient.print().printers("{id}").jobs("{id}").documents("{id}")
    .uploadData()
    .buildRequest( requestOptions )
    .post();

```