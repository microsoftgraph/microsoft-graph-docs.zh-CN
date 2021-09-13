---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8b5703a292c712ee336b25b27309628bd466fc4649f65742a4edd213c726109
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278594"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "Family"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```