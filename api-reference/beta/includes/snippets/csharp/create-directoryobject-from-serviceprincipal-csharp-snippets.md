---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2501cb7c3f78336cba37b71f1a544a33e7f945088bb6e2d7ef89152429baa0aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220211"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```