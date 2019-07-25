---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5494cb6ca61ffcfaae0c7d8258315242e0438e4b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861332"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var password = "ThisIsMyPrivatePassword";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{itemId}"]
    .CreateLink(type,scope,expirationDateTime,password,message,recipients)
    .Request()
    .PostAsync();

```