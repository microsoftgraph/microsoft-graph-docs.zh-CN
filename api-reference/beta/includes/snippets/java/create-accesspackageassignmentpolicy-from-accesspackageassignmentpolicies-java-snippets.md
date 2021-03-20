---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f69a69451503bd83c09d9b2b18226495f8c7c99
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977748"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy();
accessPackageAssignmentPolicy.accessPackageId = "56ff43fd-6b05-48df-9634-956a777fce6d";
accessPackageAssignmentPolicy.displayName = "direct";
accessPackageAssignmentPolicy.description = "direct assignments by administrator";
accessPackageAssignmentPolicy.accessReviewSettings = null;
RequestorSettings requestorSettings = new RequestorSettings();
requestorSettings.scopeType = "NoSubjects";
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

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies()
    .buildRequest()
    .post(accessPackageAssignmentPolicy);

```