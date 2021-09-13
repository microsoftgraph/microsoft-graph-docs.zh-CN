---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f907c40e5c1ada4355a375cdcfc97aaf9d09a5cb7f2ad4752e50df46427ac78
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904074"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me
    .RevokeSignInSessions()
    .Request()
    .PostAsync();

```