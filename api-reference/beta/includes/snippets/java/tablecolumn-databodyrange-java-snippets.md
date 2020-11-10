---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bc8cfd763b32fd9e47d64409a053aea96bc57f0
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980368"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .dataBodyRange()
    .buildRequest()
    .post();

```