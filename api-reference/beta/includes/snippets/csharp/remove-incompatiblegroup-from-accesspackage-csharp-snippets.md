---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d8f516d8df2420693d2e077177cba78955f32612a2d562b60270b9982fb66b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"].IncompatibleGroups["{group-id}"].Reference
    .Request()
    .DeleteAsync();

```