---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6af6b6d75925d5c21fd1616a7b07612b0fc78c1aa817be1168ef08cdfd2f5546
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378748"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments("{id}")
    .buildRequest()
    .expand("userAttribute")
    .get();

```