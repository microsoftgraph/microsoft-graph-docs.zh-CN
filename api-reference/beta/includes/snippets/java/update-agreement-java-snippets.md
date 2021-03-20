---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb105bdbccf7d185c510e3dc2461c694b2a4cd8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "displayName-value";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.identityGovernance().termsOfUse().agreements("{id}")
    .buildRequest()
    .patch(agreement);

```