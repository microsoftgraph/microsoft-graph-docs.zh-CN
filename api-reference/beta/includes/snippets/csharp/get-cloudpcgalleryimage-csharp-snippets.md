---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2196c57b0fb5724d68e3cfaa23926b63b114413e
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891107"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcGalleryImage = await graphClient.DeviceManagement.VirtualEndpoint.GalleryImages["{cloudPcGalleryImage-id}"]
    .Request()
    .GetAsync();

```