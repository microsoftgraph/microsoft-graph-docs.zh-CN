---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: db6cc981bb2b54a73589d0601585e6e4700f0c5454a6b2d1da94d5efeb25099d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageAssignments = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignments
    .Request()
    .GetAsync();

```