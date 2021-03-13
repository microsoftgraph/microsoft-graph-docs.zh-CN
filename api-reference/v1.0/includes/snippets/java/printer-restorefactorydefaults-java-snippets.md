---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6ba4fc11632d74bff9dce3d3d8356aa37d7e15fb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771797"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().printers("{printerId}")
    .restoreFactoryDefaults()
    .buildRequest()
    .post();

```