---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6d0aef725281c9501077631ec2ba08b3a92c53e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798131"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    ParentFolderId = "parentFolderId-value",
    Birthday = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    FileAs = "fileAs-value",
    DisplayName = "displayName-value",
    GivenName = "givenName-value",
    Initials = "initials-value"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Request()
    .AddAsync(contact);

```