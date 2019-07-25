---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 87cf60998b21167cfce42edea047226c8102895f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35892570"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().names("{name}")
    .range().format().fill()
    .clear()
    .buildRequest()
    .post();

```