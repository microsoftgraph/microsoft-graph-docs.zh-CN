---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d9a2d7e6af7cf54a1c885c9a7a3620c333fe497
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795018"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = new EducationalActivity
{
    Institution = new InstitutionData
    {
        Location = new PhysicalAddress
        {
            Type = PhysicalAddressType.Business,
            PostOfficeBox = null,
            Street = "12000 E Prospect Rd",
            City = "Fort Collins",
            State = "Colorado",
            CountryOrRegion = "USA",
            PostalCode = "80525"
        }
    }
};

await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .UpdateAsync(educationalActivity);

```