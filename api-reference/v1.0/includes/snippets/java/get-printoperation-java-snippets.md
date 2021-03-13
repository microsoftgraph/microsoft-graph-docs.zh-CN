---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94854f61da8e6c2a70017a3dd70e5ac53f1c037d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771377"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintOperation printOperation = graphClient.print().operations("{printOperationId}")
    .buildRequest()
    .get();

```