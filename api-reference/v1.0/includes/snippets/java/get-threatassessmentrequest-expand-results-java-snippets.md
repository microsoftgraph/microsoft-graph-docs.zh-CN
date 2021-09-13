---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2374ad9b5e264a0b4b7020bfacb819c44e871b606b6344eed3f9c1ce2b3f061c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221382"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("11922306-b25b-4605-ff0d-08d772fcf996")
    .buildRequest()
    .expand("results")
    .get();

```