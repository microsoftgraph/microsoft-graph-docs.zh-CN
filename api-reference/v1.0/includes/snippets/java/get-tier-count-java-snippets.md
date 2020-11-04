---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7ef163e178fd5d43866a020abea8e558b0d2d1da
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904300"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$orderby", "displayName "));
requestOptions.add(new QueryOption("$search", "displayName:tier"));

IGroupCollectionPage group = graphClient.users("{id}").transitiveMemberOf().microsoft.graph.group()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .get();

```