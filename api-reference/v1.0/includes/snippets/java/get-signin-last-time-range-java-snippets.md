---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29ccf2e4b4b308706d475bbe2bea8f5552f4d0b4
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905688"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("filter", "signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z"));
requestOptions.add(new QueryOption("$filter", "signInActivity/lastSignInDateTime le 2019-06-01T00:00:00Z"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .get();

```