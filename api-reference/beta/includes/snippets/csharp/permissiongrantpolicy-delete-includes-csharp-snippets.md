---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 787f882d89a7a6d0bac530d8a7e72508e97f3ac7
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Includes["198d8d6b-ecf6-47bc-a3dd-eaa2fe0544c5"]
    .Request()
    .DeleteAsync();

```