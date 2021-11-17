---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4057407679ca376f639c214c79b34673ccea08f5363d24dac168c102a4f78105
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104734"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUsers = await graphClient.IdentityProtection.RiskyUsers
    .Request()
    .Filter("riskLevel eq microsoft.graph.riskLevel'medium'")
    .GetAsync();

```