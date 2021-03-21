---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dc7c3d8189c84cfca1029d018d642648498f8a56
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970387"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Event event = new Event();
Location location = new Location();
location.displayName = "Conf Room 2";
event.location = location;

graphClient.groups("01d4ee64-15ce-491e-bad1-b91aa3223df4").calendar().events("AAMkADZlAAAAABERAAA=")
    .buildRequest()
    .patch(event);

```