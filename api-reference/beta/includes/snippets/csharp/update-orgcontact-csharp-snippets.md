---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 01fdff3219a393e9752e7f388e779d2922ffeecd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729012"
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