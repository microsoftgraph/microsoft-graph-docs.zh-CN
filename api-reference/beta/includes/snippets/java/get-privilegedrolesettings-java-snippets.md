---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1be70bbd16ff7430a4b30b983e987b81b2b867ba
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875524"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleSettings privilegedRoleSettings = graphClient.privilegedRoles("{id}").settings()
    .buildRequest()
    .get();

```