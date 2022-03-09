---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53d02d01f0b9f8b06aee2a5f7ef259639cda630cf452b0db9ba64dc203ec3721
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105271"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Id = "123456!87"
};

await graphClient.Drive.Bundles["{driveItem-id}"].Children
    .Request()
    .AddAsync(driveItem);

```