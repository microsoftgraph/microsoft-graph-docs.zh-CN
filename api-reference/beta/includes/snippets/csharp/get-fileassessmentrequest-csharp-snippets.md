---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e1119db6207e4eba51c94d22e5fc1c416277020
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867149"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["18406a56-7209-4720-a250-08d772fccdaa"]
    .Request()
    .GetAsync();

```