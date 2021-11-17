---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 103dc7b42b787c13ce798cb1195f2b27b5295d60d9cf89fef5b54bd668c66ab5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserConsentRequestCollectionPage userConsentRequests = graphClient.identityGovernance().appConsent().appConsentRequests("ee245379-e3bb-4944-a997-24115f0b8b5e").userConsentRequests()
    .buildRequest()
    .get();

```