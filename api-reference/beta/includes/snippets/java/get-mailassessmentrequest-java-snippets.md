---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 197b697fb6226f423a40f02a71fa64662df30c550c788999745e274342d067a6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104682"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("49c5ef5b-1f65-444a-e6b9-08d772ea2059")
    .buildRequest()
    .get();

```