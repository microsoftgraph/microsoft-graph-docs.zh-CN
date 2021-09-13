---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6db58ef8601bae7559d7d9ad48a1d817476a2a2bc47a3f3649c60a9246318243
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments("City")
    .buildRequest()
    .get();

```