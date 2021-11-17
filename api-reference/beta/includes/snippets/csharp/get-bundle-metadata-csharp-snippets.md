---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5d4e08ceac4ad7b7fe34d6798a7f4ac08a96521f8ef064617febc689a879d52
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Drive.Bundles["{driveItem-id}"]
    .Request()
    .GetAsync();

```