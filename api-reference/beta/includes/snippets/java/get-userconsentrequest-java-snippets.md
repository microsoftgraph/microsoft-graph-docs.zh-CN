---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8aeb84c6dd3da57c1630f502c937e721375925f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201896"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequest userConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests("acef2660-d194-4943-b927-4fe4fb5cb7e3")
    .buildRequest()
    .get();

```