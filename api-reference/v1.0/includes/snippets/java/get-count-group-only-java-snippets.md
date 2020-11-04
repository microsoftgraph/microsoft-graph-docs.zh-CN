---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 19bc8a085e4941b1e2234a2c159ad4b632d5e600
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903758"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

Int32 int32 = graphClient.servicePrincipals("{id}").memberOf().microsoft.graph.group().$count()
    .buildRequest( requestOptions )
    .get();

```