---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ded67cfc806d675c0caca8c72ec103cb4a2c445d
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var assignments = await graphClient.Education.Me.Assignments
    .Request()
    .GetAsync();

```