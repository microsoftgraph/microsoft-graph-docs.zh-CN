---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82e0f598ceadda04746fd23f97c8f7344d6f764e
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919968"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2xIdentityUserFlow = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"]
    .Request()
    .GetAsync();

```