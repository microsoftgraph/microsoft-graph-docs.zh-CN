---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 01fdff3219a393e9752e7f388e779d2922ffeecd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479850"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var orgContact = new OrgContact
{
    BusinessPhones = new List<String>()
    {
        "businessPhones-value"
    },
    City = "city-value",
    CompanyName = "companyName-value",
    Country = "country-value",
    Department = "department-value",
    DisplayName = "displayName-value"
};

await graphClient.Contacts["{id}"]
    .Request()
    .UpdateAsync(orgContact);

```