---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 932859dd73c41bdf0f0dded457d1047be31ae6d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Range", "bytes=0-72796"));

graphClient.print().printers("{id}").jobs("{id}").documents("{id}")
    .uploadData()
    .buildRequest( requestOptions )
    .post();

```