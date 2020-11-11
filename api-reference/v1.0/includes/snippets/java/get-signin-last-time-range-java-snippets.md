---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 6e1bc80ac970a026c9784bfa724bf76e913107e4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983225"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("filter", "signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .filter("signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z")
    .get();

```