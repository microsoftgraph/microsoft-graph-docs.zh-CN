---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 207ea776478b337191fe29c3f924731737a1b48e
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var projectParticipation = new ProjectParticipation
{
    Categories = new List<String>()
    {
        "categories-value"
    },
    Client = new CompanyDetail
    {
        DisplayName = "displayName-value",
        Pronunciation = "pronunciation-value",
        Department = "department-value",
        OfficeLocation = "officeLocation-value",
        Address = new PhysicalAddress
        {
            Type = PhysicalAddressType.Unknown,
            PostOfficeBox = "postOfficeBox-value",
            Street = "street-value",
            City = "city-value",
            State = "state-value",
            CountryOrRegion = "countryOrRegion-value",
            PostalCode = "postalCode-value"
        },
        WebUrl = "webUrl-value"
    },
    DisplayName = "displayName-value",
    Detail = new PositionDetail
    {
        Company = new CompanyDetail
        {
            DisplayName = "displayName-value",
            Pronunciation = "pronunciation-value",
            Department = "department-value",
            OfficeLocation = "officeLocation-value",
            Address = new PhysicalAddress
            {
                Type = PhysicalAddressType.Unknown,
                PostOfficeBox = "postOfficeBox-value",
                Street = "street-value",
                City = "city-value",
                State = "state-value",
                CountryOrRegion = "countryOrRegion-value",
                PostalCode = "postalCode-value"
            },
            WebUrl = "webUrl-value"
        },
        Description = "description-value",
        EndMonthYear = new Date(1900,1,1),
        JobTitle = "jobTitle-value",
        Role = "role-value",
        StartMonthYear = new Date(1900,1,1),
        Summary = "summary-value"
    },
    Colleagues = new List<RelatedPerson>()
    {
        new RelatedPerson
        {
            DisplayName = "displayName-value",
            Relationship = PersonRelationship.Manager,
            UserPrincipalName = "userPrincipalName-value"
        }
    },
    Sponsors = new List<RelatedPerson>()
    {
        new RelatedPerson
        {
            DisplayName = "displayName-value",
            Relationship = PersonRelationship.Manager,
            UserPrincipalName = "userPrincipalName-value"
        }
    }
};

await graphClient.Me.Profile.Projects["{id}"]
    .Request()
    .UpdateAsync(projectParticipation);

```