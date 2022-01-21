---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a907ce01298182a60b261cdb764a00c10fe4add
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62117591"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    "@odata.type" = "#microsoft.graph.educationUser"
    PrimaryRole = "String"
    MiddleName = "String"
    ExternalSource = "String"
    ExternalSourceDetail = "String"
    ResidenceAddress = @{
        "@odata.type" = "microsoft.graph.physicalAddress"
    }
    MailingAddress = @{
        "@odata.type" = "microsoft.graph.physicalAddress"
    }
    Student = @{
        "@odata.type" = "microsoft.graph.educationStudent"
    }
    Teacher = @{
        "@odata.type" = "microsoft.graph.educationTeacher"
    }
    CreatedBy = @{
        "@odata.type" = "microsoft.graph.identitySet"
    }
    AccountEnabled = "Boolean"
    AssignedLicenses = @(
        @{
            "@odata.type" = "microsoft.graph.assignedLicense"
        }
    )
    AssignedPlans = @(
        @{
            "@odata.type" = "microsoft.graph.assignedPlan"
        }
    )
    BusinessPhones = @(
        "String"
    )
    Department = "String"
    DisplayName = "String"
    GivenName = "String"
    Mail = "String"
    MailNickname = "String"
    MobilePhone = "String"
    PasswordPolicies = "String"
    PasswordProfile = @{
        "@odata.type" = "microsoft.graph.passwordProfile"
    }
    OfficeLocation = "String"
    PreferredLanguage = "String"
    ProvisionedPlans = @(
        @{
            "@odata.type" = "microsoft.graph.provisionedPlan"
        }
    )
    RefreshTokensValidFromDateTime = [System.DateTime]::Parse("String (timestamp)")
    ShowInAddressList = "Boolean"
    Surname = "String"
    UsageLocation = "String"
    UserPrincipalName = "String"
    UserType = "String"
    OnPremisesInfo = @{
        "@odata.type" = "microsoft.graph.educationOnPremisesInfo"
    }
}

New-MgEducationUser -BodyParameter $params

```