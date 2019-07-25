---
description: 自动生成的文件。 不修改
ms.openlocfilehash: bfda972ad2a967a1a147c5aba1cff515ccf32fa9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    Path = "/drive/root:/Documents"
};

var name = "Copy of LargeFolder1";

await graphClient.Me.Drive.Items["{folder-item-id}"]
    .Copy(name,parentReference)
    .Request()
    .PostAsync();

```