---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3c834521caaef77ab8b75b478a4d7020a465796
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439913"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var incompatibleGroups = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleGroups
    .Request()
    .GetAsync();

```