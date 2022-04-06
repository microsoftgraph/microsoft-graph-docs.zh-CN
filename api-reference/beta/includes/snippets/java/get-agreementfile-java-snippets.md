---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06d919f26c1d3f17f1d00e9605a87dfc34a99345
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516275"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AgreementFile agreementFile = graphClient.identityGovernance().termsOfUse().agreements("94410bbf-3d3e-4683-8149-f034e55c39dd").file()
    .buildRequest()
    .get();

```