---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44f931cb38577de8ffc7471e4c1132f654e25dfc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775932"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().shares("{printerShareId}").jobs("{printJobId}")
    .start()
    .buildRequest()
    .post();

```