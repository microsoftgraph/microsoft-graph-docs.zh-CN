---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf33184beefd03b4cf96c14235af580a1562120615444c91c09102170f53b1e8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279147"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("18406a56-7209-4720-a250-08d772fccdaa")
    .buildRequest()
    .get();

```