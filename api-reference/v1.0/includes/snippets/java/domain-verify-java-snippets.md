---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 71ece6111552913a3c8d1c987775c9a3c012a652
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883232"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.domains("{domain-name}")
    .verify()
    .buildRequest()
    .post();

```