---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 213479637477d1a48f3c1c74aace7746336cd63f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35866472"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String calculationType = "calculationType-value";

graphClient.me().drive().items("{id}").workbook().application()
    .calculate(calculationType)
    .buildRequest()
    .post();

```