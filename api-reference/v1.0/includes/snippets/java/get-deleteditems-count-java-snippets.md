---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f343d409744ee7459f97b5a6ceb75209a7b07ea
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767263"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage group = graphClient.directory().deletedItems().microsoft.graph.group()
    .buildRequest( requestOptions )
    .select("id,displayName,deletedDateTime")
    .orderBy("deletedDateTime asc")
    .get();

```