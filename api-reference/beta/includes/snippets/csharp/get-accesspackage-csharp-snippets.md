---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6e839ebadea755706180eff33221bd2d142cabfa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992851"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackage = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["{id}"]
    .Request()
    .GetAsync();

```