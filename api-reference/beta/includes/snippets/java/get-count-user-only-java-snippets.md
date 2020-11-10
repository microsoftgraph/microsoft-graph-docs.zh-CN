---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 2684e0b677db63b95d5485616846827868df51d6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48954027"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

int int32 = graphClient.groups("{id}").members().microsoft.graph.user().count()
    .buildRequest( requestOptions )
    .get();

```