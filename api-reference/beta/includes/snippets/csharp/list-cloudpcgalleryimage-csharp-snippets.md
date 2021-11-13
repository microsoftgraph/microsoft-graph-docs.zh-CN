---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a4dd5ae9b6c094d1fe8c1e9ca8823be242bcabf
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var galleryImages = await graphClient.DeviceManagement.VirtualEndpoint.GalleryImages
    .Request()
    .GetAsync();

```