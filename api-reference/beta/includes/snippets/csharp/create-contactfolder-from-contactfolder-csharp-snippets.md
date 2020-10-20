---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 791ff036fd126621b2820653633f01f25b3f8710
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612662"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```