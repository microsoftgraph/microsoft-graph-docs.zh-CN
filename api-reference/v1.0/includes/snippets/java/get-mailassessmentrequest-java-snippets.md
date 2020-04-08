---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d78a78c0f57247012c18abae2dbb5de84ed942dd
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858801"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("49c5ef5b-1f65-444a-e6b9-08d772ea2059")
    .buildRequest()
    .get();

```