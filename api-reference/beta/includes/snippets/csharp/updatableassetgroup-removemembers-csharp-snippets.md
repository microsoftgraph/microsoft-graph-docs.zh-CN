---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a68af2ad9a95c76de4b5ac8ba3db474241eb7b6c5ec4adb39fab86dd58819f8f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158443"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assets = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.AzureADDevice
    {
        Id = "String (identifier)"
    }
};

await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .RemoveMembers(assets)
    .Request()
    .PostAsync();

```