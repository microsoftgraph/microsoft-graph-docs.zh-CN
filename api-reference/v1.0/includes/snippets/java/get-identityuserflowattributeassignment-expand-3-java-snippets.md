---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 414a24760aa1493389b1c8ec7307f97223ee0e5f
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920717"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = graphClient.identity().b2xUserFlows("{id}").userAttributeAssignments("{id}")
    .buildRequest()
    .expand("userAttribute")
    .get();

```