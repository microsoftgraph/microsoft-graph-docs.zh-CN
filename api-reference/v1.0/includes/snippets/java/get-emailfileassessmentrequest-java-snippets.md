---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e0d220a846aac5c81fe4c936eb2e0d512ee6220
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858807"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("ab2ad9b3-2213-4091-ae0c-08d76ddbcacf")
    .buildRequest()
    .get();

```