---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 203fe66aee83dbfea506f66a2bd677c6efef2a9cc195dfb8a04a016ca2fe6f08
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333723"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .expand("principal")
    .get();

```