---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3257d0e2c134e27a7da2821c78aaf5b3bbb2aa74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771419"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String reason = "String";

graphClient.print().printers("{printerId}").jobs("{printJobId}")
    .abort(reason)
    .buildRequest()
    .post();

```