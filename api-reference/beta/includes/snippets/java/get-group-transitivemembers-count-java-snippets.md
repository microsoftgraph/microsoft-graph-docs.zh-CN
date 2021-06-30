---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a711dabbbf615986f2cf9869f2b7385899872959
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207169"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

int int32 = graphClient.groups("{id}").transitiveMembers().count()
    .buildRequest( requestOptions )
    .get();

```