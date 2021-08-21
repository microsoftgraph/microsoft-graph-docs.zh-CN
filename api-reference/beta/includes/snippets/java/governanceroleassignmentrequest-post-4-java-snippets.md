---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef83e0c1ae72ad67a1afba10b8c3ef477f3960a65f214b42f8a488bac3ce3f60
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105763"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "65bb4622-61f5-4f25-9d75-d0e20cf92019";
governanceRoleAssignmentRequest.resourceId = "e5e7d29d-5465-45ac-885f-4716a5ee74b5";
governanceRoleAssignmentRequest.subjectId = "74765671-9ca4-40d7-9e36-2f4a570608a6";
governanceRoleAssignmentRequest.assignmentState = "Eligible";
governanceRoleAssignmentRequest.type = "AdminRemove";

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```