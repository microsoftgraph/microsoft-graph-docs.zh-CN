---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 30df7ebfcecd04b1235137adab49ec425f1aa6f7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201858"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequest userConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests("filterByCurrentUser(on='reviewer')")
    .buildRequest()
    .filter(" (status eq 'Completed')")
    .get();

```