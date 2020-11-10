---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3605bdaa636bb7fff3a3242a20a0908b44e5adb2
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968168"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTaskDefinition printTaskDefinition = graphClient.print().taskDefinitions("fab143fd-ee61-4358-8558-2c7dee953982")
    .buildRequest()
    .get();

```