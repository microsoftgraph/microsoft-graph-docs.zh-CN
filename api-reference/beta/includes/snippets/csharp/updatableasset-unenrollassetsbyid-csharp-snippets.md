---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a5a1da9089e9b4182943e8fcb4358b4d164809b528084736b5d50f4bac28db3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333306"
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