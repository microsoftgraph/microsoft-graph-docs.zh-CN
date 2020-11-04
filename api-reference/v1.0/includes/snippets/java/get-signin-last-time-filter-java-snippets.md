---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 79d6405f45472eb81254fef8ac06a86ebbe6b0e4
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905682"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new QueryOption("$filter", "startswith(displayName,'Eric'),"));

IUserCollectionPage users = graphClient.users()
    .buildRequest( requestOptions )
    .select("displayName,signInActivity")
    .get();

```