---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44aaaf62fb9eb65dfc79d8eece43216f94fe0c3e934ece3fb106f4e7308ae87b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162411"
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