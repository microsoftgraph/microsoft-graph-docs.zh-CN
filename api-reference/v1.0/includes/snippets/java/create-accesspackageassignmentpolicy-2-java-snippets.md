---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de4dcc7e6ef9ab480c7d63c169f3f2cbdb86451d
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209625"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessPackageAssignmentPolicy accessPackageAssignmentPolicy = new AccessPackageAssignmentPolicy();
accessPackageAssignmentPolicy.displayName = "policy for external access requests";
accessPackageAssignmentPolicy.description = "policy for users from connected organizations to request access, with two stages of approval.";
accessPackageAssignmentPolicy.allowedTargetScope = AllowedTargetScope.ALL_CONFIGURED_CONNECTED_ORGANIZATION_USERS;
LinkedList<SubjectSet> specificAllowedTargetsList = new LinkedList<SubjectSet>();
accessPackageAssignmentPolicy.specificAllowedTargets = specificAllowedTargetsList;
ExpirationPattern expiration = new ExpirationPattern();
expiration.type = ExpirationPatternType.NO_EXPIRATION;
accessPackageAssignmentPolicy.expiration = expiration;
AccessPackageAssignmentRequestorSettings requestorSettings = new AccessPackageAssignmentRequestorSettings();
requestorSettings.enableTargetsToSelfAddAccess = true;
requestorSettings.enableTargetsToSelfUpdateAccess = true;
requestorSettings.enableTargetsToSelfRemoveAccess = true;
requestorSettings.allowCustomAssignmentSchedule = false;
requestorSettings.enableOnBehalfRequestorsToAddAccess = false;
requestorSettings.enableOnBehalfRequestorsToUpdateAccess = false;
requestorSettings.enableOnBehalfRequestorsToRemoveAccess = false;
LinkedList<SubjectSet> onBehalfRequestorsList = new LinkedList<SubjectSet>();
requestorSettings.onBehalfRequestors = onBehalfRequestorsList;
accessPackageAssignmentPolicy.requestorSettings = requestorSettings;
AccessPackageAssignmentApprovalSettings requestApprovalSettings = new AccessPackageAssignmentApprovalSettings();
requestApprovalSettings.isApprovalRequiredForAdd = true;
requestApprovalSettings.isApprovalRequiredForUpdate = false;
LinkedList<AccessPackageApprovalStage> stagesList = new LinkedList<AccessPackageApprovalStage>();
AccessPackageApprovalStage stages = new AccessPackageApprovalStage();
stages.durationBeforeAutomaticDenial = DatatypeFactory.newInstance().newDuration("P14D");
stages.isApproverJustificationRequired = false;
stages.isEscalationEnabled = false;
stages.durationBeforeEscalation = DatatypeFactory.newInstance().newDuration("PT0S");
LinkedList<SubjectSet> primaryApproversList = new LinkedList<SubjectSet>();
InternalSponsors primaryApprovers = new InternalSponsors();
primaryApproversList.add(primaryApprovers);
stages.primaryApprovers = primaryApproversList;
LinkedList<SubjectSet> fallbackPrimaryApproversList = new LinkedList<SubjectSet>();
SingleUser fallbackPrimaryApprovers = new SingleUser();
fallbackPrimaryApprovers.userId = "7deff43e-1f17-44ef-9e5f-d516b0ba11d4";
fallbackPrimaryApproversList.add(fallbackPrimaryApprovers);
GroupMembers fallbackPrimaryApprovers1 = new GroupMembers();
fallbackPrimaryApprovers1.groupId = "1623f912-5e86-41c2-af47-39dd67582b66";
fallbackPrimaryApproversList.add(fallbackPrimaryApprovers1);
stages.fallbackPrimaryApprovers = fallbackPrimaryApproversList;
LinkedList<SubjectSet> escalationApproversList = new LinkedList<SubjectSet>();
stages.escalationApprovers = escalationApproversList;
LinkedList<SubjectSet> fallbackEscalationApproversList = new LinkedList<SubjectSet>();
stages.fallbackEscalationApprovers = fallbackEscalationApproversList;
stagesList.add(stages);
AccessPackageApprovalStage stages1 = new AccessPackageApprovalStage();
stages1.durationBeforeAutomaticDenial = DatatypeFactory.newInstance().newDuration("P14D");
stages1.isApproverJustificationRequired = false;
stages1.isEscalationEnabled = false;
stages1.durationBeforeEscalation = DatatypeFactory.newInstance().newDuration("PT0S");
LinkedList<SubjectSet> primaryApproversList1 = new LinkedList<SubjectSet>();
stages1.primaryApprovers = primaryApproversList1;
LinkedList<SubjectSet> fallbackPrimaryApproversList1 = new LinkedList<SubjectSet>();
SingleUser fallbackPrimaryApprovers2 = new SingleUser();
fallbackPrimaryApprovers2.userId = "46184453-e63b-4f20-86c2-c557ed5d5df9";
fallbackPrimaryApproversList1.add(fallbackPrimaryApprovers2);
GroupMembers fallbackPrimaryApprovers3 = new GroupMembers();
fallbackPrimaryApprovers3.groupId = "1623f912-5e86-41c2-af47-39dd67582b66";
fallbackPrimaryApproversList1.add(fallbackPrimaryApprovers3);
stages1.fallbackPrimaryApprovers = fallbackPrimaryApproversList1;
LinkedList<SubjectSet> escalationApproversList1 = new LinkedList<SubjectSet>();
stages1.escalationApprovers = escalationApproversList1;
LinkedList<SubjectSet> fallbackEscalationApproversList1 = new LinkedList<SubjectSet>();
stages1.fallbackEscalationApprovers = fallbackEscalationApproversList1;
stagesList.add(stages1);
requestApprovalSettings.stages = stagesList;
accessPackageAssignmentPolicy.requestApprovalSettings = requestApprovalSettings;
AccessPackage accessPackage = new AccessPackage();
accessPackage.id = "a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b";
accessPackageAssignmentPolicy.accessPackage = accessPackage;

graphClient.identityGovernance().entitlementManagement().assignmentPolicies()
    .buildRequest()
    .post(accessPackageAssignmentPolicy);

```