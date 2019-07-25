---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a2e67c41bbe291c8198071fff49ec5a4f49c0705
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889615"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuditLogRoot auditLogRoot = graphClient.auditLogs()
    .buildRequest()
    .get();

```