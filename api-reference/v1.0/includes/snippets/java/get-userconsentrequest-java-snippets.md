---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 045c55ba72aee7dec39544dbbb6c7e1e4daeae7a19ef7e54d58fc038c4f8591a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279311"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequest userConsentRequest = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests("acef2660-d194-4943-b927-4fe4fb5cb7e3")
    .buildRequest()
    .get();

```