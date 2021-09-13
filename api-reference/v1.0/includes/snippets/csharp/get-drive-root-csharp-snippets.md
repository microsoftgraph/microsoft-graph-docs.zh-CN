---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 068c80bcb6a44946b7807f3d2c80e79e002a2a50eea9a254b047e9d275176590
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Root
    .Request()
    .GetAsync();

```