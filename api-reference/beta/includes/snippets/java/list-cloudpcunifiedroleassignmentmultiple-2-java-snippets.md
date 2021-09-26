---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 894f617ec9c712bab1e56ac0354c85d681c2a7bdedb9be076dbfaaacf658ffeb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentMultipleCollectionPage roleAssignments = graphClient.roleManagement().cloudPC().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq 'b5c08161-a7af-481c-ace2-a20a69a48fb1'")
    .get();

```