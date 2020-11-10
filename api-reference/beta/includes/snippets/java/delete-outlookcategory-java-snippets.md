---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8324d84c27fa47e08473fcaafa6866f5f8f02818
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48972884"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().outlook().masterCategories("4b1c2495-54c9-4a5e-90a2-0ab0b31987d8")
    .buildRequest()
    .delete();

```