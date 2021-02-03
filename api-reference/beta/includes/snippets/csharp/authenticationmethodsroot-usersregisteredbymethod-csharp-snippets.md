---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 848297b0dfc10e4d8ffd0a3b18b27201f32ffbca
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092368"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userRegistrationMethodSummary = await graphClient.Reports.AuthenticationMethods
    .UsersRegisteredByMethod(.all,.all)
    .Request()
    .GetAsync();

```