---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f605987307e3a3a28522ec8fa3286d686afb9684d4cc5ee6ee6a8160a57cac44
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219414"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var ids = new List<String>()
{
    "String",
    "String",
    "String"
};

var memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"]
    .AddMembersById(ids,memberEntityType)
    .Request()
    .PostAsync();

```