---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3a665d5dadd3e4311cb05193d97e02c421984df
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779335"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .GetAsync();

```