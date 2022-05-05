---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc5534413efc4eb423a070e89013a8199bd4a7d6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204202"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

UserCollectionPage user = graphClient.groups("{id}").transitiveMembers().microsoft.graph.user()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .orderBy("displayName")
    .get();

```