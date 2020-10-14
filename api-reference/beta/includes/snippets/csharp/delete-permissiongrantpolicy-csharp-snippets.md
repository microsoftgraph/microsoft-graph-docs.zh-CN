---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5324b04827fd154c308f7592ba3b514ca520f8
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"]
    .Request()
    .DeleteAsync();

```