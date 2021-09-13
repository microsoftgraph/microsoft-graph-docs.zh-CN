---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbc2e6643d13f6f64e30c00ed39658106307c7d876366255605cc45dc00f988f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57334002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .Request()
    .GetAsync();

```