---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4a3b2292c724797540518b9e6ed840ae3f69beeb0fa15e13b79cbad3ec6421e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332816"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AppConsentRequestFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().appConsent().appConsentRequests()
    .filterByCurrentUser(AppConsentRequestFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .filter("userConsentRequests/any(u:u/status eq 'InProgress')")
    .get();

```