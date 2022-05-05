---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bff250aa507457618ba74433b316915e9bdb8bc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209986"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage groups = graphClient.groups()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .orderBy("displayName")
    .top(1)
    .get();

```