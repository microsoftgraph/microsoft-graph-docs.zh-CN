---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e628845ad059bff51c62d06e9ba73c0d357403d4
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921384"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProviders = await graphClient.Identity.IdentityProviders
    .Request()
    .GetAsync();

```