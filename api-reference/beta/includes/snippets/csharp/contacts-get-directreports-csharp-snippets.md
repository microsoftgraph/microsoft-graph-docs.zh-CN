---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 958ab1606c2a1766aee6f314e3ac22d8a2dad19c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directReports = await graphClient.Contacts["{id}"].DirectReports
    .Request()
    .GetAsync();

```