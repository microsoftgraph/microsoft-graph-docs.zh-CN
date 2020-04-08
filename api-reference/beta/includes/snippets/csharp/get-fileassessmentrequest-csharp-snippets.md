---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1119db6207e4eba51c94d22e5fc1c416277020
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "40867149"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["18406a56-7209-4720-a250-08d772fccdaa"]
    .Request()
    .GetAsync();

```