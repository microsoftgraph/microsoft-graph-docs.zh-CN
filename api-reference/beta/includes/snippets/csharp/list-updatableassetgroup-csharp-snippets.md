---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d04e73a67ded7d9dac85b1e219f91326247aef11cb50bb47ee6cddad1d45539e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var updatableAssets = await graphClient.Admin.Windows.Updates.UpdatableAssets
    .Request()
    .Filter("isof('microsoft.graph.windowsUpdates.updatableAssetGroup')")
    .GetAsync();

```