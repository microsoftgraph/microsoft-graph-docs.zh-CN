---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 09a1f9e0bdac7dbb60c97e0d580b4e9f5de3c716
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871001"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUser riskyUser = graphClient.riskyUsers("c2b6c2b9-dddc-acd0-2b39-d519d803dbc3")
    .buildRequest()
    .get();

```