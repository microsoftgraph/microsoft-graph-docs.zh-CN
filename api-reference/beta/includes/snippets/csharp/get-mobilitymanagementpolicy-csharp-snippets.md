---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 601f6242064723954bd7e4e70b8bbc2b7b2ef118
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440291"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var mobilityManagementPolicy = await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"]
    .Request()
    .GetAsync();

```