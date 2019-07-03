---
description: 自动生成的文件。 不修改
ms.openlocfilehash: dd9af7e5b3a02d00b164e2b2aaa2b40cd62dbd02
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = "Binary data for the image"

await graphClient.Me.Photo.Content
    .Request()
    .PutAsync(Stream);

```