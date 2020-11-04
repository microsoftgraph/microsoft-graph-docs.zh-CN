---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8104b62d3b557879109af14080e6d63eee389622
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905949"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

IOrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest( requestOptions )
    .get();

```