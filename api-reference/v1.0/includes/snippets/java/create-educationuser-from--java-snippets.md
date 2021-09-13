---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f52947eb7b64781f7cb79aafa84084f2815a5fd28065787754d91d6b7619b28c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57107048"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.primaryRole = EducationUserRole.STUDENT;
educationUser.middleName = "String";
educationUser.externalSource = EducationExternalSource.SIS;
educationUser.externalSourceDetail = "String";
PhysicalAddress residenceAddress = new PhysicalAddress();
educationUser.residenceAddress = residenceAddress;
PhysicalAddress mailingAddress = new PhysicalAddress();
educationUser.mailingAddress = mailingAddress;
EducationStudent student = new EducationStudent();
educationUser.student = student;
EducationTeacher teacher = new EducationTeacher();
educationUser.teacher = teacher;
IdentitySet createdBy = new IdentitySet();
educationUser.createdBy = createdBy;
educationUser.accountEnabled = false;
LinkedList<AssignedLicense> assignedLicensesList = new LinkedList<AssignedLicense>();
AssignedLicense assignedLicenses = new AssignedLicense();
assignedLicensesList.add(assignedLicenses);
educationUser.assignedLicenses = assignedLicensesList;
LinkedList<AssignedPlan> assignedPlansList = new LinkedList<AssignedPlan>();
AssignedPlan assignedPlans = new AssignedPlan();
assignedPlansList.add(assignedPlans);
educationUser.assignedPlans = assignedPlansList;
LinkedList<String> businessPhonesList = new LinkedList<String>();
businessPhonesList.add("String");
educationUser.businessPhones = businessPhonesList;
educationUser.department = "String";
educationUser.displayName = "String";
educationUser.givenName = "String";
educationUser.mail = "String";
educationUser.mailNickname = "String";
educationUser.mobilePhone = "String";
educationUser.passwordPolicies = "String";
PasswordProfile passwordProfile = new PasswordProfile();
educationUser.passwordProfile = passwordProfile;
educationUser.officeLocation = "String";
educationUser.preferredLanguage = "String";
LinkedList<ProvisionedPlan> provisionedPlansList = new LinkedList<ProvisionedPlan>();
ProvisionedPlan provisionedPlans = new ProvisionedPlan();
provisionedPlansList.add(provisionedPlans);
educationUser.provisionedPlans = provisionedPlansList;
educationUser.refreshTokensValidFromDateTime = OffsetDateTimeSerializer.deserialize("String (timestamp)");
educationUser.showInAddressList = false;
educationUser.surname = "String";
educationUser.usageLocation = "String";
educationUser.userPrincipalName = "String";
educationUser.userType = "String";
EducationOnPremisesInfo onPremisesInfo = new EducationOnPremisesInfo();
educationUser.onPremisesInfo = onPremisesInfo;

graphClient.education().users()
    .buildRequest()
    .post(educationUser);

```