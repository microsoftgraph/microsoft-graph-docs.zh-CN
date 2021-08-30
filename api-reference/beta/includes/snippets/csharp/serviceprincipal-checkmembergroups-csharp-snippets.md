---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e3cd6dbd0c6912def3ee468206ebfa8007336f8a936a6b427f6805d440c8c8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216011"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "groupIds-value"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```