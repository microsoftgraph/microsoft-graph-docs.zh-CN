---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a6ae05b0d53b14067daf1b9b6fba985fdf7727c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var subjectRightsRequest = new SubjectRightsRequestObject
{
    Type = SubjectRightsRequestType.Export,
    DataSubjectType = DataSubjectType.Customer,
    Regulations = new List<String>()
    {
        "String"
    },
    DisplayName = "String",
    Description = "String",
    InternalDueDateTime = DateTimeOffset.Parse("String (timestamp)"),
    DataSubject = new DataSubject
    {
        FirstName = "String",
        LastName = "String",
        Email = "String",
        Residency = "String",
        AdditionalData = new Dictionary<string, object>()
        {
            {"phoneNumber", "String"},
            {"SSN", "String"}
        }
    }
};

await graphClient.Privacy.SubjectRightsRequests
    .Request()
    .AddAsync(subjectRightsRequest);

```