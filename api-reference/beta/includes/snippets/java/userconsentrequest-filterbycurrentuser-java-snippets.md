---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4592024f6a982e42c10d048d24df74161d2d64f5c1ac02c147cc4144499ea6d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903024"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequestFilterByCurrentUserCollectionPage filterByCurrentUser = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests()
    .filterByCurrentUser(UserConsentRequestFilterByCurrentUserParameterSet
        .newBuilder()
        .withOn('reviewer')
        .build())
    .buildRequest()
    .filter(" (status eq 'Completed')")
    .get();

```