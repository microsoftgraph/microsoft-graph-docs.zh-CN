---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2386449040b9430cb734b5b70895d4072573fc5a14a337888b174bba962f32b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378372"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var addMembers = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var removeMembers = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var addExclusions = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

var removeExclusions = new List<Microsoft.Graph.WindowsUpdates.UpdatableAsset>()
{
    new Microsoft.Graph.WindowsUpdates.UpdatableAsset
    {
        Id = "String (identifier)"
    }
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"].Audience
    .UpdateAudience(addMembers,removeMembers,addExclusions,removeExclusions)
    .Request()
    .PostAsync();

```