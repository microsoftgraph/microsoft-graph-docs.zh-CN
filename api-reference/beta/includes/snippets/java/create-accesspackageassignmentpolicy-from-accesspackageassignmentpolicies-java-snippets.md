---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e27ba40f2e4c00e0e853f97c1d0e2ef6e37552642ef3de8b65178e7b3afdbc96
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104193"
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