---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d4be1d97c1e89b719ecacce2d49dfd302d94ad7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976308"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.additionalInformation = "additionalInformation-after-update";
tiIndicator.confidence = 42;
tiIndicator.description = "description-after-update";

graphClient.security().tiIndicators("{id}")
    .buildRequest( requestOptions )
    .patch(tiIndicator);

```