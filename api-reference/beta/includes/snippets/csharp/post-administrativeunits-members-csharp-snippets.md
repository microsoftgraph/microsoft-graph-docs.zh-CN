---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64343e83446f1be3eada6b37c5d2cef56c96c52d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.AdministrativeUnits["{administrativeUnit-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```