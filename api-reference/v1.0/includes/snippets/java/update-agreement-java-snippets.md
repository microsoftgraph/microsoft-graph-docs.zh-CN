---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c77e1929ad27b6a4e1e597a0b7c90c8a06749abd69556883166f94ee288c9b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57328903"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Agreement agreement = new Agreement();
agreement.displayName = "Sample ToU display name";
agreement.isViewingBeforeAcceptanceRequired = true;

graphClient.identityGovernance().termsOfUse().agreements("093b947f-8363-4979-a47d-4c52b33ee1be")
    .buildRequest()
    .patch(agreement);

```