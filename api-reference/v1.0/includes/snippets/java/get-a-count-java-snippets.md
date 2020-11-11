---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 889fc35eb99fd9886a7ae5752f8549facb66f1fc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983820"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .filter("startswith(displayName,'a'),")
    .orderBy("displayName ")
    .top(1)
    .get();

```