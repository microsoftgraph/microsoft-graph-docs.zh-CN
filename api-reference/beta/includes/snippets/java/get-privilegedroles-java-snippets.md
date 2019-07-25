---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1d5db62969e03cb0f1ee4b3408b270757047258d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875818"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleCollectionPage privilegedRoles = graphClient.privilegedRoles()
    .buildRequest()
    .get();

```