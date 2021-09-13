---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d621e3738931cfa31c95cfcf2fa2dfad65f5ab9c44ecdafd139188e0319a8fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106207"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teamwork.WorkforceIntegrations["{workforceIntegration-id}"]
    .Request()
    .DeleteAsync();

```