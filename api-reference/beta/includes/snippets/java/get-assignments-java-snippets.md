---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 384cef0dbbc1a69c32256523d8ab65f3e95c74c5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875845"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentCollectionPage assignments = graphClient.privilegedRoles("{id}").assignments()
    .buildRequest()
    .get();

```