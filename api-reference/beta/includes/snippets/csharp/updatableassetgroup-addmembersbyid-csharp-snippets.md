---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8127b23e0cf29278d840f4f3938a7ea7f1de2838
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239485"
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