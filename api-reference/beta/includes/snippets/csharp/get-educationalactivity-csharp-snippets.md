---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dc6e74be63860e262ea8f0196fefdbc6f7cd623
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803088"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationalActivity = await graphClient.Me.Profile.EducationalActivities["{educationalActivity-id}"]
    .Request()
    .GetAsync();

```