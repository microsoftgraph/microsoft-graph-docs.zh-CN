---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48c3f32873a31ca3d3ee7b1a9a9275fd9a7ae2c6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618790"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var secureScoreControlProfile = new SecureScoreControlProfile
{
    ControlStateUpdates = "controlStateUpdates-value"
};

await graphClient.Security.SecureScoreControlProfiles["AdminMFA"]
    .Request()
    .UpdateAsync(secureScoreControlProfile);

```