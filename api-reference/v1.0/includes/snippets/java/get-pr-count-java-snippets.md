---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 1fbc6b8f2afb2e12339d367686e4df366be54913
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983462"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Pr"));

IUserCollectionPage user = graphClient.groups("{id}").members().microsoft.graph.user()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .orderBy("displayName ")
    .get();

```