---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c2632754f847180622a45953fb9ca68dbfbfc686
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875860"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRole privilegedRole = graphClient.privilegedRoles("{id}")
    .buildRequest()
    .get();

```