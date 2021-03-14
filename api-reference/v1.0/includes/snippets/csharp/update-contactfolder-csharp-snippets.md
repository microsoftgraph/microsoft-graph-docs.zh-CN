---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0a478c481db7d688ca5472f7fdca86ac203f7e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782900"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "parentFolderId-value",
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .UpdateAsync(contactFolder);

```