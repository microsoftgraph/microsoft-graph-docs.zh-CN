---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0b1ee519187a9da15ee1b4a9472870f676a8a15
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952120"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy();
accessPackageAssignmentPolicy.id = "b2eba9a1-b357-42ee-83a8-336522ed6cbf";
accessPackageAssignmentPolicy.accessPackageId = "1b153a13-76da-4d07-9afa-c6c2b1f2e824";
accessPackageAssignmentPolicy.displayName = "All Users";
accessPackageAssignmentPolicy.description = "All users can request for access to the directory.";
accessPackageAssignmentPolicy.isDenyPolicy = false;
accessPackageAssignmentPolicy.canExtend = false;
accessPackageAssignmentPolicy.durationInDays = 365;
RequestorSettings requestorSettings = new RequestorSettings();
requestorSettings.scopeType = "AllExistingDirectorySubjects";
requestorSettings.acceptRequests = true;
LinkedList<UserSet> allowedRequestorsList = new LinkedList<UserSet>();
requestorSettings.allowedRequestors = allowedRequestorsList;
accessPackageAssignmentPolicy.requestorSettings = requestorSettings;
ApprovalSettings requestApprovalSettings = new ApprovalSettings();
requestApprovalSettings.isApprovalRequired = false;
requestApprovalSettings.isApprovalRequiredForExtension = false;
requestApprovalSettings.isRequestorJustificationRequired = false;
requestApprovalSettings.approvalMode = "NoApproval";
LinkedList<ApprovalStage> approvalStagesList = new LinkedList<ApprovalStage>();
requestApprovalSettings.approvalStages = approvalStagesList;
accessPackageAssignmentPolicy.requestApprovalSettings = requestApprovalSettings;
accessPackageAssignmentPolicy.accessReviewSettings = null;

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("b2eba9a1-b357-42ee-83a8-336522ed6cbf")
    .buildRequest()
    .put(accessPackageAssignmentPolicy);

```