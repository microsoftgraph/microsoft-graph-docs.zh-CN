---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e2debeace6c8cd305a96181d40a46778d9ec423f1b91d0c9d4b35b27895afbbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{group-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```