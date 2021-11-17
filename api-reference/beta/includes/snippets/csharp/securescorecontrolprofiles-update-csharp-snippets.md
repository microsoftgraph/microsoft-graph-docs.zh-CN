---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a81a89ea03ea9678a93c31ed0428a371bc9fcc53cb9a46a7080f3e3586c32741
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163925"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    ControlStateUpdates = "controlStateUpdates-value"
};

await graphClient.Security.SecureScoreControlProfiles["{secureScoreControlProfile-id}"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```