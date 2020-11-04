---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 008cc57df63cd46fd2297e51ab0f9fbee8e040ca
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903654"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$filter", "startswith(displayName,'a'),"));
requestOptions.add(new QueryOption("$orderby", "displayName "));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .top(1)
    .get();

```