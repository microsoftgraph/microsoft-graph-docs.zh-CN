---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d130b941ee4b1360ac82ae0552aa521e1c558272
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962806"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("723c35be-8b5a-47ae-29c0-08d76ddb7f5b")
    .buildRequest()
    .get();

```