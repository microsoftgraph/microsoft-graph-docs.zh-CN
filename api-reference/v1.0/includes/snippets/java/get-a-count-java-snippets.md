---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 055627c4c2a42c256991e05c640e306eadb50e49
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083306"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

ServicePrincipalCollectionPage servicePrincipals = graphClient.servicePrincipals()
    .buildRequest( requestOptions )
    .filter("startswith(displayName, 'a')")
    .orderBy("displayName")
    .top(1)
    .get();

```