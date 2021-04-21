---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e584305cfcc39a822e071088ffb4bd4f591b2aa8
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919932"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].IdentityProviders
    .Request()
    .GetAsync();

```