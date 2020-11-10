---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c5d40823a24d37b26b20ff8275248269269a5c3a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979823"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{id}").taskTriggers()
    .buildRequest()
    .get();

```