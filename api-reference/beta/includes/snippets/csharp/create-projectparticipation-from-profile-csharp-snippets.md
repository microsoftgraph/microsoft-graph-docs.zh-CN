---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 061a67cffd8b5d294d48dc851d94f409c72de235
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996498"
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

await graphClient.Me.Profile.Projects
    .Request()
    .AddAsync(projectParticipation);

```