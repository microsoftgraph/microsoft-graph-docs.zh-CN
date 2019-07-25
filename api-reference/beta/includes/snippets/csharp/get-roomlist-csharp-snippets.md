---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b57383ba45fdd1dbb4179ab492154a82710668b4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876838"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["bldg1@contoso.com"]
    .Request()
    .GetAsync();

```