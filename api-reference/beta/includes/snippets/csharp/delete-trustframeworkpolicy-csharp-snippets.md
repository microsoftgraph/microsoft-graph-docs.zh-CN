---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9347ecf60601cea3766351f62a253ebccd77b5c5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35480236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.Policies["B2C_1A_SocialAndLocalAccounts_Base"]
    .Request()
    .DeleteAsync();

```