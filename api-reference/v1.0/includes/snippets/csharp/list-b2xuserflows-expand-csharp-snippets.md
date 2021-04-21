---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75ed3faa0b923c5dc3de681eb220ea6b6293e576
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xUserFlows = await graphClient.Identity.B2xUserFlows
    .Request()
    .Expand("identityProviders")
    .GetAsync();

```