---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbc0f42c44b78e10f3927e64200900125f27f6f8
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428843"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = "Binary data for the image"

await graphClient.Me.Photo.Content
    .Request()
    .PutAsync(stream);

```