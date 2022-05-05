---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 631e1e9d3e6bdc29c8d5ef85c0185c746d92dee3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilitySchedules = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules
    .Request()
    .GetAsync();

```