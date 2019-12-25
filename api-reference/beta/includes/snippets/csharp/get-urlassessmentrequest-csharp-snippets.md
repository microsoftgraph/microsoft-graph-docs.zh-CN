---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b424490c0d170088f28d2f83c907d03644c84ed
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["723c35be-8b5a-47ae-29c0-08d76ddb7f5b"]
    .Request()
    .GetAsync();

```