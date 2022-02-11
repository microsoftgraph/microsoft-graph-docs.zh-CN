---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f457b1ed6de6f67e7db259cacfaee44c926119db
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62530581"
---
```powershell

Import-Module Microsoft.Graph.Education

$params = @{
    RelatedContacts = @(
        @{
            DisplayName = "Father Time"
            EmailAddress = "father@time.com"
            MobilePhone = "4251231234"
            Relationship = "guardian"
            AccessConsent = $true
        }
        @{
            DisplayName = "Mother Nature"
            EmailAddress = "mother@nature.co.uk"
            MobilePhone = "3251231234"
            Relationship = "parent"
            AccessConsent = $true
        }
    )
}

Update-MgEducationUser -EducationUserId $educationUserId -BodyParameter $params

```