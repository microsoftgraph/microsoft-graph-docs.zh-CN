---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb7fb59ea10b2139def1a4f5ed3680df89e9f078
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240692"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updateCategory = Microsoft.Graph.WindowsUpdates.UpdateCategory.Feature;

var memberEntityType = "#microsoft.graph.windowsUpdates.azureADDevice";

var ids = new List<String>()
{
    "String",
    "String",
    "String"
};

await graphClient.Admin.Windows.Updates.UpdatableAssets
    .UnenrollAssetsById(updateCategory,memberEntityType,ids)
    .Request()
    .PostAsync();

```