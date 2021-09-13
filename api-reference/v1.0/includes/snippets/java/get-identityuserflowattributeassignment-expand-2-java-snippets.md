---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70ca51b2106aa7665b60330906cf20940c66760786068d53aca83a0105f18e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903555"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignmentCollectionPage userAttributeAssignments = graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments()
    .buildRequest()
    .expand("userAttribute")
    .get();

```