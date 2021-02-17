---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cc9f20144cefef0d088afe8cae054b99f67459e
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["d69179bf-f4a4-41a9-a9de-249c0f2efb1d"].Branding
    .Request()
    .DeleteAsync();

```