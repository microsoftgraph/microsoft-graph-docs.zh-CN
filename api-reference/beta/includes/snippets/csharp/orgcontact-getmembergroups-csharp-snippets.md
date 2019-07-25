---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d04a6c93a19d9c343bc529a3a82a632eff4f0377
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35721046"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.Contacts["{id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```