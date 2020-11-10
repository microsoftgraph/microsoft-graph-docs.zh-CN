---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c8547eeb9a274d97cbc42c267ab18d2a33813898
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970428"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedRoleAssignmentCollectionWithReferencesPage assignments = graphClient.privilegedRoles("{id}").assignments()
    .buildRequest()
    .get();

```