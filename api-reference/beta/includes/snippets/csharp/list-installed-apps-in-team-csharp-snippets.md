---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51586e79e19ac08fdeef77fabe36f1725a80e2d3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690733"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Teams["6903fa93-605b-43ef-920e-77c4729f8258"].InstalledApps
    .Request()
    .GetAsync();

```