---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e84b53d2d6fbc6a483eb3feff137ce0f1df53016f5f8f0c6c0872f9a181ce302
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Identity.UserFlows["{identityUserFlow-id}"]
    .Request()
    .DeleteAsync();

```