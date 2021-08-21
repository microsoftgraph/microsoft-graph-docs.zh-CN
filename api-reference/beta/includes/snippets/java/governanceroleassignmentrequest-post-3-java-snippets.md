---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 892fa7183372901ffb8fa717da80eb00e5cd512588383c95f6207c7db1c1be76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleAssignmentRequest governanceRoleAssignmentRequest = new GovernanceRoleAssignmentRequest();
governanceRoleAssignmentRequest.roleDefinitionId = "bc75b4e6-7403-4243-bf2f-d1f6990be122";
governanceRoleAssignmentRequest.resourceId = "fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735";
governanceRoleAssignmentRequest.subjectId = "918e54be-12c4-4f4c-a6d3-2ee0e3661c51";
governanceRoleAssignmentRequest.assignmentState = "Active";
governanceRoleAssignmentRequest.type = "UserRemove";
governanceRoleAssignmentRequest.reason = "Deactivate the role";
governanceRoleAssignmentRequest.linkedEligibleRoleAssignmentId = "cb8a533e-02d5-42ad-8499-916b1e4822ec";

graphClient.privilegedAccess("azureResources").roleAssignmentRequests()
    .buildRequest()
    .post(governanceRoleAssignmentRequest);

```