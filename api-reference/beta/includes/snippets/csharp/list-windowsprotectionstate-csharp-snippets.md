---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94b052ff371afe78906f00c4fcd07e2e32de76c3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442293"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var windowsProtectionStates = await graphClient.TenantRelationships.ManagedTenants.WindowsProtectionStates
    .Request()
    .GetAsync();

```