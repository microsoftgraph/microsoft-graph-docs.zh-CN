---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c355a577a5c6cc5010a61f2eea7b67a90daf644b
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998935"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Applications["{id}"].Owners.References
    .Request()
    .AddAsync(directoryObject);

```