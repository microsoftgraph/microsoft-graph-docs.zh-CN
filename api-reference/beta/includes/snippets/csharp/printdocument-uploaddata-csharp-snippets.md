---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e17d8dec0b7fd3f9c06ba412abb3a5168e8e8dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"].Documents["{printDocument-id}"]
    .UploadData()
    .Request()
    .Header("Range","bytes=0-72796")
    .PostAsync();

```