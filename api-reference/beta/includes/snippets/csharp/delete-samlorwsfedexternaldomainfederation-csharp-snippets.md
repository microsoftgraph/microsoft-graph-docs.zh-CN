---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1101baa35f39176c3f29b25d0f676221b86cd134
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Directory.FederationConfigurations["{identityProviderBase-id}"]
    .Request()
    .DeleteAsync();

```