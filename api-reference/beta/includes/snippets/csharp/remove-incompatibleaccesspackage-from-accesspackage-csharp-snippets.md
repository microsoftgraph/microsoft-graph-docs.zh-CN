---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbb5318c3bcc7cf1a726a7cc51e4d8bd20b16b19
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleAccessPackages["{accessPackage-id}"].Reference
    .Request()
    .DeleteAsync();

```