---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9cd20c85734d1c77b9c96fa559a57f175081907c
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903653"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

Int32 int32 = graphClient.groups("{id}").members().microsoft.graph.user().$count()
    .buildRequest( requestOptions )
    .get();

```