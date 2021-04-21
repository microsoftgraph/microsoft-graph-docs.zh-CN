---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73ef752e192e571caecb92f6d6c83fb5d2c27711
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920464"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Identity.B2xUserFlows["{b2xIdentityUserFlow-id}"].Languages["{userFlowLanguageConfiguration-id}"].DefaultPages["{userFlowLanguagePage-id}"].Content
    .Request()
    .GetAsync();

```