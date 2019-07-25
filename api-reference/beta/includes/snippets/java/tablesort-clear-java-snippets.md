---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f72a1905058c56554cf03d32326099a3ee9bad6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868461"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").sort()
    .clear()
    .buildRequest()
    .post();

```