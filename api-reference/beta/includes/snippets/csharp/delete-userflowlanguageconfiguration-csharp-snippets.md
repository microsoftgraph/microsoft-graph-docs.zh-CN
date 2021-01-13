---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65563b493015dd7ba87622cf9b78530d7bac3522
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844959"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.B2cUserFlows["B2C_1_Customer"].Languages["es-ES"]
    .Request()
    .DeleteAsync();

```