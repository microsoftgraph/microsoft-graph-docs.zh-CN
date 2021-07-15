---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d3327205e3db7e81c045694dd76f298577c5e6e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440412"
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