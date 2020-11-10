---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 611400aa968b86b6a733d4d5e453f2f1ea044fd5
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979122"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .headerRowRange()
    .buildRequest()
    .post();

```