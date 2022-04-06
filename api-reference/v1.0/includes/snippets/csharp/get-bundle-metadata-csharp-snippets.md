---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e7827bdc630569b3b7535de4f58d0e597832fe0
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757985"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Drive.Bundles["{driveItem-id}"]
    .Request()
    .GetAsync();

```