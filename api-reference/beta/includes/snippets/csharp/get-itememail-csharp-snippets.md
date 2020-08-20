---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be45f1cee68f4680c774a6e57b96ff9c855094e2
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820030"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemEmail = await graphClient.Users["{userId}"].Profile.Emails["{id}"]
    .Request()
    .GetAsync();

```