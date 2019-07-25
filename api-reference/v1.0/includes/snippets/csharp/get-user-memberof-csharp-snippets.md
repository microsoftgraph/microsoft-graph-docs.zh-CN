---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0f0de65547b6beba04649ea5058fde1aef706934
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894894"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Devices["{id}"].MemberOf
    .Request()
    .GetAsync();

```