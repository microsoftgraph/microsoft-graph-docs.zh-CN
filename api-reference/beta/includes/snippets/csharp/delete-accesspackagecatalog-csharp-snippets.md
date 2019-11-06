---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4cd240a340b26df3d21efdb7c4afb6dac042b6ab
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["{id}"]
    .Request()
    .DeleteAsync();

```