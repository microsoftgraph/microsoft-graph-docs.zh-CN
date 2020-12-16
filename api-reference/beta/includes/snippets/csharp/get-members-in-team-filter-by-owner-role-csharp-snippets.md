---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b52eebdd9caf63aef6742333938f4a967ccb09c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690821"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062"].Members
    .Request()
    .Filter("roles/any(r:r eq 'owner')")
    .GetAsync();

```