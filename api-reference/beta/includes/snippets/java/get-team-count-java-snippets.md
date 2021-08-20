---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b13f791aa0fe388a8b80481a29f9d20437612f2b0ae5bb33cc5353954f8ec45
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Team"));

ServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest( requestOptions )
    .get();

```