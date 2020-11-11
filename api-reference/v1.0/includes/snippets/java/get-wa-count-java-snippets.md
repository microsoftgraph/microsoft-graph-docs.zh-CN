---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 6cf47893a525b74b5d0d21be30883eacc4cbf63d
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983909"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));
requestOptions.add(new QueryOption("$search", "displayName:wa"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .orderBy("displayName ")
    .get();

```