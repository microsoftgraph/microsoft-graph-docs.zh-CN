---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb181b6027d60067129afc0425af6213a3e9996c
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["5b649834-7412-4cce-9e69-176e95a394f5"].Teamwork.InstalledApps["NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk"]
    .Upgrade()
    .Request()
    .PostAsync();

```