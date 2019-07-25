---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 63b02eb56ff643f34d88ceba91a61fceadbcf5d3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871071"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItem riskyUserHistoryItem = graphClient.riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69")
    .buildRequest()
    .get();

```