---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f71749d80ee777232370777364b76260f8c4b572
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment
{
    UserInputType = IdentityUserFlowAttributeInputType.TextBox
};

await graphClient.Identity.B2cUserFlows["{b2cIdentityUserFlowId}"].UserAttributeAssignments["{id}"]
    .Request()
    .UpdateAsync(identityUserFlowAttributeAssignment);

```