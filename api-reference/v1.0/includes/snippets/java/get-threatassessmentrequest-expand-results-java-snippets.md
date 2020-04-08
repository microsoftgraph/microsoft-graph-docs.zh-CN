---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a9b9850568cf0f777bc03fda6cedbd61df6b3a6a
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858860"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("11922306-b25b-4605-ff0d-08d772fcf996")
    .buildRequest()
    .expand("results")
    .get();

```