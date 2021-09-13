---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 895c4c9334c9dbaf7660fb63e5aa7e43804c249b208a2722f372a70ad30a7772
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163277"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = new EducationUser
{
    PrimaryRole = EducationUserRole.Student,
    MiddleName = "String",
    ExternalSource = EducationExternalSource.Sis,
    ExternalSourceDetail = "String",
    ResidenceAddress = new PhysicalAddress
    {
    },
    MailingAddress = new PhysicalAddress
    {
    },
    Student = new EducationStudent
    {
    },
    Teacher = new EducationTeacher
    {
    },
    CreatedBy = new IdentitySet
    {
    },
    AccountEnabled = false,
    AssignedLicenses = new List<AssignedLicense>()
    {
        new AssignedLicense
        {
        }
    },
    AssignedPlans = new List<AssignedPlan>()
    {
        new AssignedPlan
        {
        }
    },
    BusinessPhones = new List<String>()
    {
        "String"
    },
    Department = "String",
    DisplayName = "String",
    GivenName = "String",
    Mail = "String",
    MailNickname = "String",
    MobilePhone = "String",
    PasswordPolicies = "String",
    PasswordProfile = new PasswordProfile
    {
    },
    OfficeLocation = "String",
    PreferredLanguage = "String",
    ProvisionedPlans = new List<ProvisionedPlan>()
    {
        new ProvisionedPlan
        {
        }
    },
    RefreshTokensValidFromDateTime = DateTimeOffset.Parse("String (timestamp)"),
    ShowInAddressList = false,
    Surname = "String",
    UsageLocation = "String",
    UserPrincipalName = "String",
    UserType = "String",
    OnPremisesInfo = new EducationOnPremisesInfo
    {
    }
};

await graphClient.Education.Users
    .Request()
    .AddAsync(educationUser);

```