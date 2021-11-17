---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a5c9f113c95308a5ed4f2de07d619d7f7b94af64593c2d0c93eb043deb95ba9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278745"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedPermissionClassifications = await graphClient.ServicePrincipals["{servicePrincipal-id}"].DelegatedPermissionClassifications
    .Request()
    .GetAsync();

```