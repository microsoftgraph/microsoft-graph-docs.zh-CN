---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d2a512367d61d184e558662cc0691832e4726046
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Tags["{teamworkTag-id}"]
    .Request()
    .DeleteAsync();

```