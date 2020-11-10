---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: f1d800137c7f57ac9b0eebce91f57d58e59b4358
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979468"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

int int32 = graphClient.users("{id}").memberOf().count()
    .buildRequest( requestOptions )
    .get();

```