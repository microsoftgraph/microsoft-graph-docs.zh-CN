---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6382f9976fff5540f900d00414407a9d85ed04b8
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970527"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().messages("{id}")
    .unsubscribe()
    .buildRequest()
    .post();

```