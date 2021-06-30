---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e99ab4dcc35f4536ffa2bd8932b4784d321a1dd
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210826"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Users["{user-id}"].TransitiveReports.$count
    .Request()
    .GetAsync();

```