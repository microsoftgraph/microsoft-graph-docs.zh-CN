---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b1889226018b27d7ad0d163072421d8b446d9d80
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892955"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().tables("{id|name}").columns("{id|name}")
    .totalRowRange()
    .buildRequest()
    .post();

```