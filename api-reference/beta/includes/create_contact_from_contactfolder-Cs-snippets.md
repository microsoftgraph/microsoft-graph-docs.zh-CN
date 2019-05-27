---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d61190bb3ac103c723f6e88cd7f16f9c1898cd5f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457113"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    ParentFolderId = "parentFolderId-value",
    Birthday = "2016-10-19T10:37:00Z",
    FileAs = "fileAs-value",
    DisplayName = "displayName-value",
    GivenName = "givenName-value",
    Initials = "initials-value"
};

await graphClient.Me.ContactFolders["{id}"].Contacts
    .Request()
    .AddAsync(contact);

```