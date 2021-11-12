---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa5acae9c8b039ccebd6406c0841c5c8ec64863973ab108b8f547443d3d1e4b1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Applications["{application-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```