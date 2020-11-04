---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d4c7dbed3777ea31b622d54dd5149b2159809e1
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905491"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Team"));

IServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest( requestOptions )
    .get();

```