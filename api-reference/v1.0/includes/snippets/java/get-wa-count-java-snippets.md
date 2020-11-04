---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22d34687c50b77523ef7db19c55da5c3d7fb47dc
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905687"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$orderby", "displayName "));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .get();

```