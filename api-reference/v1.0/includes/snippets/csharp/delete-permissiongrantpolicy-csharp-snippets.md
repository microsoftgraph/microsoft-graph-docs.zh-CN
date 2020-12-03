---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5a5324b04827fd154c308f7592ba3b514ca520f8
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524327"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"]
    .Request()
    .DeleteAsync();

```