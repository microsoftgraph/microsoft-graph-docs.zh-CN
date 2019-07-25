---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8674dd49aaa6d4a7d3251a15f1f9efeee025160b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive
    .Search('{search-query}')
    .Request()
    .GetAsync();

```