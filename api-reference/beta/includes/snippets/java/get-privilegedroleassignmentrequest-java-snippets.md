---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c98081efebbf1e793c4007bd1194500b2125e2cc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875580"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentRequestCollectionPage privilegedRoleAssignmentRequests = graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .get();

```