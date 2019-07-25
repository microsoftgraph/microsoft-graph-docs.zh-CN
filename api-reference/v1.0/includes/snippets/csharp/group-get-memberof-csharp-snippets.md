---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c85dcb04ed8b011e933d95488421ffc39d936884
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35889128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.Groups["{id}"].MemberOf
    .Request()
    .GetAsync();

```