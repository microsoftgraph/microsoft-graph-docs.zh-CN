---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b811646c6880fba44bd000987ba86d7ca67efc539c78f5593e3f52e181484fad
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274003"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "alexd@contoso.com"
};

await graphClient.Groups["{group-id}"].AcceptedSenders.References
    .Request()
    .AddAsync(directoryObject);

```