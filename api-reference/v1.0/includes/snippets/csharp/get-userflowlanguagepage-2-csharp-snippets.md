---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e5fa1773d7124fddc6967e3fab907413120c8324
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920537"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var overridesPages = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].OverridesPages
    .Request()
    .GetAsync();

```