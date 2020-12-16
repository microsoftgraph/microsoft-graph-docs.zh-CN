---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8a48c173b65de24683f6f42209ccff2b0e571b0
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690551"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var presence = await graphClient.Communications.Presences["dc74d9bb-6afe-433d-8eaa-e39d80d3a647"]
    .Request()
    .GetAsync();

```