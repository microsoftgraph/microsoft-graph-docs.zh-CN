---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6382f9976fff5540f900d00414407a9d85ed04b8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879380"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .unsubscribe()
    .buildRequest()
    .post();

```