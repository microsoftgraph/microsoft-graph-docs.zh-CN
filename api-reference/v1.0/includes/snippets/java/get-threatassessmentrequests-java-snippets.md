---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddfb26818f89836f9028ac6578efb2ce09e8a9f6
ms.sourcegitcommit: 9edfcf99706c8490cd5832a1c706a88a89e24db1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2020
ms.locfileid: "42815952"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IThreatAssessmentRequestCollectionPage threatAssessmentRequests = graphClient.informationProtection().threatAssessmentRequests()
    .buildRequest()
    .get();

```