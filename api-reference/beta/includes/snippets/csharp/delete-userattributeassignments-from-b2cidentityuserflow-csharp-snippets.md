---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b0abd7e169d49b9adbbb132ef051a1b87b815d7
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689540"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["{id}"].UserAttributeAssignments["{id}"]
    .Request()
    .DeleteAsync();

```