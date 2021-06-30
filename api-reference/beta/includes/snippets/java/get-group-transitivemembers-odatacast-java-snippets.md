---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60a31b362c506c8d4d86fca00e0aab416dde5b46
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

GroupCollectionPage group = graphClient.groups("{id}").transitiveMembers().microsoft.graph.group()
    .buildRequest( requestOptions )
    .get();

```