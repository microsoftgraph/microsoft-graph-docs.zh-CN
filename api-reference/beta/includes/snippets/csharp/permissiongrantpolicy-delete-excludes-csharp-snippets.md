---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71367c86d21e774e344045d9624eb7c07d31ba6d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460329"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Excludes["6a846635-3e70-4a10-821e-512a0db93cbd"]
    .Request()
    .DeleteAsync();

```