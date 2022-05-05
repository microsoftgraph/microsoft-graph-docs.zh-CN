---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f4f9e8165543665e036a44055f4ee4246f1c2b9
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209605"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy();
accessPackageAssignmentPolicy.displayName = "New Policy";
accessPackageAssignmentPolicy.description = "policy for assignment";
accessPackageAssignmentPolicy.allowedTargetScope = AllowedTargetScope.NOT_SPECIFIED;
LinkedList<SubjectSet> specificAllowedTargetsList = new LinkedList<SubjectSet>();
accessPackageAssignmentPolicy.specificAllowedTargets = specificAllowedTargetsList;
ExpirationPattern expiration = new ExpirationPattern();
expiration.endDateTime = OffsetDateTimeSerializer.deserialize("null");
expiration.duration = DatatypeFactory.newInstance().newDuration("null");
expiration.type = ExpirationPatternType.NO_EXPIRATION;
accessPackageAssignmentPolicy.expiration = expiration;
AccessPackageAssignmentRequestorSettings requestorSettings = new AccessPackageAssignmentRequestorSettings();
requestorSettings.enableTargetsToSelfAddAccess = false;
requestorSettings.enableTargetsToSelfUpdateAccess = false;
requestorSettings.enableTargetsToSelfRemoveAccess = false;
requestorSettings.allowCustomAssignmentSchedule = true;
requestorSettings.enableOnBehalfRequestorsToAddAccess = false;
requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false;
requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false;
LinkedList<SubjectSet> onBehalfRequestorsList = new LinkedList<SubjectSet>();
requestorSettings.onBehalfRequestors = onBehalfRequestorsList;
accessPackageAssignmentPolicy.requestorSettings = requestorSettings;
AccessPackageAssignmentApprovalSettings requestApprovalSettings = new AccessPackageAssignmentApprovalSettings();
requestApprovalSettings.isApprovalRequiredForAdd = false;
requestApprovalSettings.isApprovalRequiredForUpdate = false;
LinkedList<AccessPackageApprovalStage> stagesList = new LinkedList<AccessPackageApprovalStage>();
requestApprovalSettings.stages = stagesList;
accessPackageAssignmentPolicy.requestApprovalSettings = requestApprovalSettings;
AccessPackage accessPackage = new AccessPackage();
accessPackage.id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b";
accessPackageAssignmentPolicy.accessPackage = accessPackage;

graphClient.identityGovernance().entitlementManagement().assignmentPolicies()
    .buildRequest()
    .post(accessPackageAssignmentPolicy);

```