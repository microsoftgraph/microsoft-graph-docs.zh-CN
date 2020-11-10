---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bbb9b264514b560ece8fd3634fffa60f1b5dfa9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971121"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}")
    .convertToRange()
    .buildRequest()
    .post();

```