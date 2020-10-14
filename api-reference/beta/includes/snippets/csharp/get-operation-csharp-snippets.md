---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b741bb050e791ad54cd82f82fbbd536ba50b325
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var longRunningOperation = await graphClient.Users["{id | userPrincipalName}"].Authentication.Operations["{id}"]
    .Request()
    .GetAsync();

```