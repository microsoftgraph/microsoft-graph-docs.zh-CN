---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb128c264f2f08b9df8c0ec257ff0f4a8e143f2b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203270"
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