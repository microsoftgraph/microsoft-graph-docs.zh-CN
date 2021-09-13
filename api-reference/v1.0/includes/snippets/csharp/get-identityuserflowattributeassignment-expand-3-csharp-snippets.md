---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1211d1d5603a77d746dc6c3e02e46dc97600c43538e7cb64bc394a9a42b327a8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378752"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].UserAttributeAssignments["{identityUserFlowAttributeAssignment-id}"]
    .Request()
    .Expand("userAttribute")
    .GetAsync();

```