---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c2488ea9822e019684622ba1115b6e4005553abd
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44900289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

using var stream = new System.IO.MemoryStream(Encoding.UTF8.GetBytes("Binary data for the image"));

await graphClient.Me.Photo.Content
    .Request()
    .PutAsync(stream);

```