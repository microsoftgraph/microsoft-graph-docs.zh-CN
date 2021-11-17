---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95f0ece5f669f35bd4b15cc1101a33665560c1787a5b2f02c14baac9acae1a07
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104683"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["{threatAssessmentRequest-id}"]
    .Request()
    .Expand("results")
    .GetAsync();

```