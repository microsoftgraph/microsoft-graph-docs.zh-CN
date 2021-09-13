---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc85dc86495939a15b11fbdc37bf5494aae16ce3cf82c633e1552717d89d65b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333234"
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