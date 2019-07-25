---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9347ecf60601cea3766351f62a253ebccd77b5c5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724364"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.TrustFramework.Policies["B2C_1A_SocialAndLocalAccounts_Base"]
    .Request()
    .DeleteAsync();

```