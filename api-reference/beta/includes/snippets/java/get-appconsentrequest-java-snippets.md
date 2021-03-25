---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f0cdc214595b2eaad2293349fb3319dfb28e964
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201718"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequest appConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("af330b30-dd59-4482-a848-0fd81b0438ed")
    .buildRequest()
    .get();

```