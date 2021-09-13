---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ce2f61a0572934091c1ad2ad56810f13d86634c20e4f68f7a1a926843e0c7b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var threatAssessmentRequest = await graphClient.InformationProtection.ThreatAssessmentRequests["{threatAssessmentRequest-id}"]
    .Request()
    .GetAsync();

```