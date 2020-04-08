---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b424490c0d170088f28d2f83c907d03644c84ed
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858814"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["723c35be-8b5a-47ae-29c0-08d76ddb7f5b"]
    .Request()
    .GetAsync();

```