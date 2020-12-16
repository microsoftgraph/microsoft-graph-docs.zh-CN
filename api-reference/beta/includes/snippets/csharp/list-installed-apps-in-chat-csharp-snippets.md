---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 86f95d91151b3ce71cd3866e3a027feb3365f5de
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689860"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var installedApps = await graphClient.Chats["19:d65713bc498c4a428c71ef9353e6ce20@thread.v2"].InstalledApps
    .Request()
    .GetAsync();

```