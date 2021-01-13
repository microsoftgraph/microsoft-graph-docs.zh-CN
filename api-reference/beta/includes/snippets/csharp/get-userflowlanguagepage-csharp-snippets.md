---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f8d7b375d98a2b34bd69517e79debacd77d6132
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844833"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Identity.B2cUserFlows["B2C_1_Customer"].Languages["en"].DefaultPages["idpselections"].Content
    .Request()
    .GetAsync();

```