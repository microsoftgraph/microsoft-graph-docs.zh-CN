---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00bbd75e6b684bae977e206a522b33bbeb08728b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239288"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAssets = await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .Filter("isof('microsoft.graph.windowsUpdates.azureADDevice')")
    .GetAsync();

```