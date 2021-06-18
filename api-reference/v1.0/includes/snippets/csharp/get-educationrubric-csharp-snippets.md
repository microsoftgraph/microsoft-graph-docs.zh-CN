---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3a665d5dadd3e4311cb05193d97e02c421984df
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990932"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationRubric = await graphClient.Education.Me.Rubrics["{educationRubric-id}"]
    .Request()
    .GetAsync();

```