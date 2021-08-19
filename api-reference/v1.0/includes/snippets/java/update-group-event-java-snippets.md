---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a5f2a4afac328fe030b5820a3a1b1a2e09445f3242c5627db078dc1e9a53f62
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104573"
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