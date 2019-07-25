---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 99e198b94e9018f1c88f913ef068dfc7a5678c3a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870053"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.ServicePrincipals["{id}"].CreatedObjects
    .Request()
    .GetAsync();

```