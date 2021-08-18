---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f362b695d1b4e5e7d15b64c0f5710a9810b943c
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384119"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:Pr"));

UserCollectionPage user = graphClient.groups("{id}").members().microsoft.graph.user()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .orderBy("displayName")
    .get();

```