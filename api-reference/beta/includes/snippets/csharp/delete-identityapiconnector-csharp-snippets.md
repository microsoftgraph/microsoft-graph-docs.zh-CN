---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96f99bdacb0330d77eb9c6860ac66e6ff725c072
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808563"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.ApiConnectors["{identityApiConnector-id}"]
    .Request()
    .DeleteAsync();

```