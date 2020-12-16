---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c26d2d3fe8652f25d5d684225c0322f2741d84d
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690823"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var members = await graphClient.Teams["ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062"].Members
    .Request()
    .GetAsync();

```