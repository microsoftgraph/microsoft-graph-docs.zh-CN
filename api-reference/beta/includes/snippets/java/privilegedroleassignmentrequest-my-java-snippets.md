---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e0e515add0b78f1366c29f4d451cf9f1b901c836
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875560"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentRequestCollectionPage my = graphClient.privilegedRoleAssignmentRequests()
    .my()
    .buildRequest()
    .get();

```