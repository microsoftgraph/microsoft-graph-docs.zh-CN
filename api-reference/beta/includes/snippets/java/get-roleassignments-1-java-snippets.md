---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec0227a34a0d85857f3b5fb2cfc8b99994af6bbe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959060"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUnifiedRoleAssignmentCollectionPage roleAssignments = graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .filter("roleDefinitionId eq '62e90394-69f5-4237-9190-012177145e10'")
    .expand("principal")
    .get();

```