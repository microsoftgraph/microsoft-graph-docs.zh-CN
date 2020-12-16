---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd9dd9cae69b9296e9e9f3adc25f7355d43a421d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690949"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Users["5b649834-7412-4cce-9e69-176e95a394f5"].Teamwork.InstalledApps
    .Request()
    .Expand("teamsAppDefinition")
    .GetAsync();

```