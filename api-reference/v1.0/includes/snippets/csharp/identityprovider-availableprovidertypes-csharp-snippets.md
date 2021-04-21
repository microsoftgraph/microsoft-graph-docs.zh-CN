---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d313a3e4334097f8cb19040816ec4606e17e404
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availableProviderTypes = await graphClient.IdentityProviders
    .AvailableProviderTypes()
    .Request()
    .GetAsync();

```