---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 587e41c8e6b489ccb298894a7eb0aaf558794e67
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42858813"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("18406a56-7209-4720-a250-08d772fccdaa")
    .buildRequest()
    .get();

```