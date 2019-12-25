---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e5fe9f88385a7181e49adb1248847ea6a79b734
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["11922306-b25b-4605-ff0d-08d772fcf996"]
    .Request()
    .Expand("results")
    .GetAsync();

```