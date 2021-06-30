---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06dd5022e60c138b1f417206960326f89eea9f50
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210071"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tags = await graphClient.Teams["{team-id}"].Tags
    .Request()
    .GetAsync();

```