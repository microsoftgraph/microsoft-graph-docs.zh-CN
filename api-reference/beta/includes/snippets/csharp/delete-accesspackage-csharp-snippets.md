---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb1f81694a3b58fa51d202b555d71f48524e10507d51830adcc82751ea0fb04d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{accessPackage-id}"]
    .Request()
    .DeleteAsync();

```