---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f551f31676007db576199eb2d59ac3f866df49909957ffbc06a29c61bf2d290
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220789"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Planner.All
    .Delta()
    .Request()
    .GetAsync();

```