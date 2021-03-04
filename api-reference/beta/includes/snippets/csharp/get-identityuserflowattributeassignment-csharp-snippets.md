---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a105ee5b8f5c27e878c58cb87ecbfcbbfbdd4df4
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "50435159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAttributeAssignments = await graphClient.Identity.B2xUserFlows["{id}"].UserAttributeAssignments
    .Request()
    .GetAsync();

```