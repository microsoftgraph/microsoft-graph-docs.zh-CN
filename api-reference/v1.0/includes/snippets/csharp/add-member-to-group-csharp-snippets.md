---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd3e06207a73ee859bbd0bb9a1c73b2d8035fd75
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413329"
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