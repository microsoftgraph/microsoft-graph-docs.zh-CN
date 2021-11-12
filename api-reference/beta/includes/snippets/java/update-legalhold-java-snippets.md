---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aab3ea0281d3836e3764c972b1e3baaa0b42c8900b842eb18afb0db585bf5f38
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278786"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHold legalHold = new LegalHold();
legalHold.description = "This is a description for a legalHold";

graphClient.compliance().ediscovery().cases("{caseId}").legalHolds("{legalholdId}")
    .buildRequest()
    .patch(legalHold);

```