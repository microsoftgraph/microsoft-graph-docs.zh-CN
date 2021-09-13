---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a514e632172b8cf23bedade7e6c9cff06596cc75422b263adcc4339b121d95d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{sharedDriveItem-id}"].DriveItem
    .Request()
    .GetAsync();

```