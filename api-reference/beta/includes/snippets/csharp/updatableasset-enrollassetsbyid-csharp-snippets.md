---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94d0f7f431e3221b0c8d23af78ffc4b062f0d96a9d448a70af814abe9071670c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220469"
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
    .EnrollAssetsById(updateCategory,memberEntityType,ids)
    .Request()
    .PostAsync();

```