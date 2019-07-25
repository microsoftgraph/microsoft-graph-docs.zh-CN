---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5b20fdb7edec9ad1043124fe06af853c3424611c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856927"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.appRoleAssignments("{id}")
    .buildRequest()
    .delete();

```