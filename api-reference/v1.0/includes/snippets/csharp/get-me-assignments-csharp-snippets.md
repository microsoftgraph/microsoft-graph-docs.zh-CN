---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded67cfc806d675c0caca8c72ec103cb4a2c445d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111073"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Me.Assignments
    .Request()
    .GetAsync();

```