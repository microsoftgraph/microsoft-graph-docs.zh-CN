---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb128c264f2f08b9df8c0ec257ff0f4a8e143f2b
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368841"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

OrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest( requestOptions )
    .filter("startswith(displayName,'A')")
    .orderBy("displayName")
    .top(1)
    .get();

```