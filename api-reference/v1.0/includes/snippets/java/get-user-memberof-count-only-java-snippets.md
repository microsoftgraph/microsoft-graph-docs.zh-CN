---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00494e90078c093d0ec1597d7b0cb5660dad1b64
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905860"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("ConsistencyLevel", "eventual"));

Int32 int32 = graphClient.users("{id}").memberOf().$count()
    .buildRequest( requestOptions )
    .get();

```