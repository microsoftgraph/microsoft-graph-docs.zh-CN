---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95be6ef97e68c2d06c7c365009739011bd30a8de
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776870"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Printer printer = graphClient.print().printers("{printerId}")
    .buildRequest()
    .get();

```