---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 215943080ce8f200375a6056cf510e297c37c857
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061033"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleAssignment unifiedRoleAssignment = new UnifiedRoleAssignment();
unifiedRoleAssignment.principalId = "6b937a9d-c731-465b-a844-2d5b5368c161";
unifiedRoleAssignment.roleDefinitionId = "9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3";
unifiedRoleAssignment.directoryScopeId = "/661e1310-bd76-4795-89a7-8f3c8f855bfc";

graphClient.roleManagement().directory().roleAssignments()
    .buildRequest()
    .post(unifiedRoleAssignment);

```