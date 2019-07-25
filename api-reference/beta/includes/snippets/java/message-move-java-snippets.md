---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bc59e46ef37dd01712e227cc65fc2ea560b58274
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879463"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "deleteditems";

graphClient.me().messages("AAMkADhAAATs28OAAA=")
    .move(destinationId)
    .buildRequest()
    .post();

```