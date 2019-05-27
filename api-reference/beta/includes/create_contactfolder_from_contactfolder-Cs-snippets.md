---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 791ff036fd126621b2820653633f01f25b3f8710
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457078"
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