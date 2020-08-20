---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36d66d2d72814cfe9220c1a6c268453b6f7239bb
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemPublication = await graphClient.Me.Profile.Publications["{id}"]
    .Request()
    .GetAsync();

```