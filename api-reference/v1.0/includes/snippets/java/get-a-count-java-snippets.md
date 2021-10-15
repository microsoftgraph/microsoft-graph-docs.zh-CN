---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb128c264f2f08b9df8c0ec257ff0f4a8e143f2b
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2021
ms.locfileid: "59766224"
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