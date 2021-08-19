---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc805e069d6c9997059781992ad7de49dc7dc5792a22520acbe2a0fd8024024
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219484"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:tier"));

UserCollectionPage user = graphClient.groups("{id}").transitiveMembers().microsoft.graph.user()
    .buildRequest( requestOptions )
    .select("displayName,id")
    .orderBy("displayName")
    .get();

```