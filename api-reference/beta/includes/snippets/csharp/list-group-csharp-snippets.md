---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7cabb609d2f0141cf42b8862555d356323196bd0
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440963"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includedGroups = await graphClient.Policies.MobileDeviceManagementPolicies["{mobilityManagementPolicy-id}"].IncludedGroups
    .Request()
    .GetAsync();

```