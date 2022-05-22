---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4d6ec5bbc89f8b031fb4efdf0ed6d077cf3af58
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629351"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getStorageAccounts = await graphClient.DeviceManagement.VirtualEndpoint.Snapshots
    .GetStorageAccounts("cb6ad4c4-8a17-4245-a644-e4436b1ee204")
    .Request()
    .GetAsync();

```