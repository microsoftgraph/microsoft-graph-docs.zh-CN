---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 873dd998a5974e167c6b2e2230b6d8977d2ae73c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875740"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignment privilegedRoleAssignment = graphClient.privilegedRoleAssignments("{id}")
    .buildRequest()
    .get();

```