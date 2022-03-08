---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d462b0bb7a22652221f316cc03f2933d762de4a8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336667"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

User user = graphClient.me()
    .buildRequest( requestOptions )
    .expand("manager($levels=max;$select=id,displayName)")
    .select("id,displayName")
    .get();

```