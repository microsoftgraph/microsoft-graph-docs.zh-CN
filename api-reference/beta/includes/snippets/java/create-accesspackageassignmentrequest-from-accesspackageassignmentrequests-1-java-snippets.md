---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83303f8c80e75b73b61a5b16bb9e7e180cae1104
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943203"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentRequest accessPackageAssignmentRequest = new AccessPackageAssignmentRequest();
accessPackageAssignmentRequest.requestType = "AdminAdd";
AccessPackageAssignment accessPackageAssignment = new AccessPackageAssignment();
accessPackageAssignment.targetId = "46184453-e63b-4f20-86c2-c557ed5d5df9";
accessPackageAssignment.assignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8";
accessPackageAssignment.accessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b";
accessPackageAssignmentRequest.accessPackageAssignment = accessPackageAssignment;

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentRequests()
    .buildRequest()
    .post(accessPackageAssignmentRequest);

```