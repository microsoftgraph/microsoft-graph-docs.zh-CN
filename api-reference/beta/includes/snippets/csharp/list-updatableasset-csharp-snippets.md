---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9245453bbf67036cc7e47089de34443004b6e8e7
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "61004293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Admin.Windows.Updates.UpdatableAssets["{windowsUpdates.updatableAsset-id}"].Members
    .Request()
    .GetAsync();

```