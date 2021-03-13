---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7596fc85594e5b8068a0438e1670bbc059dff4e3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774934"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "Sample ToU display name";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.identityGovernance().termsOfUse().agreements("093b947f-8363-4979-a47d-4c52b33ee1be")
    .buildRequest()
    .patch(agreement);

```