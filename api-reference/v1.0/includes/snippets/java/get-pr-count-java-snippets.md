---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 23a0f5d6a6c8f7f38afeaae35d9fd0762bcbc902
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903648"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$orderby", "displayName "));
requestOptions.add(new QueryOption("$search", "displayName:Pr"));

IUserCollectionPage user = graphClient.groups("{id}").members().microsoft.graph.user()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .get();

```