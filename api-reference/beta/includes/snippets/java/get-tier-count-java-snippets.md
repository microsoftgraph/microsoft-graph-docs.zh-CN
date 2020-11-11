---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: ab0c2e54748a0232d64632b09d20e45fcb9f2b4b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48953895"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:tier"));

IGroupCollectionPage group = graphClient.users("{id}").transitiveMemberOf().microsoft.graph.group()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .orderBy("displayName ")
    .get();

```