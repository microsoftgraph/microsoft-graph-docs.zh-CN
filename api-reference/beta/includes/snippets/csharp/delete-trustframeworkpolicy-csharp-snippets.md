---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9347ecf60601cea3766351f62a253ebccd77b5c5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.Policies["B2C_1A_SocialAndLocalAccounts_Base"]
    .Request()
    .DeleteAsync();

```