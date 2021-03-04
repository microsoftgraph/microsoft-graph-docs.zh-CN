---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f14ca745916aa8b9d5e2d91bb6fecd6d163da79
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435163"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2xUserFlows["{id}"].UserAttributeAssignments
    .Request()
    .Expand("userAttribute")
    .GetAsync();

```