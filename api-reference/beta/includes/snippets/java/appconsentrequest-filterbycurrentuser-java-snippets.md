---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 040d3880e9818486d99d774d6b37a21f71779390
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573116"
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