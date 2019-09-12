---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ae9252ced46b9b186abafa8df78deb0c09ed52d
ms.sourcegitcommit: d8a58221ed1f2b7b7073fd621da4737e11ba53c5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/11/2019
ms.locfileid: "36845965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    ParentFolderId = "parentFolderId-value",
    Birthday = DateTimeOffset.Parse("datetime-value"),
    FileAs = "fileAs-value",
    DisplayName = "displayName-value",
    GivenName = "givenName-value",
    Initials = "initials-value"
};

await graphClient.Me.ContactFolders["{id}"].Contacts
    .Request()
    .AddAsync(contact);

```