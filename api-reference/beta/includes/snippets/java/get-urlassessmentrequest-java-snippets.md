---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8aba7d396bbc1b6057d3779d59970dd65756a62dc5a22617a4ff1962bf77fb66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903042"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("723c35be-8b5a-47ae-29c0-08d76ddb7f5b")
    .buildRequest()
    .get();

```