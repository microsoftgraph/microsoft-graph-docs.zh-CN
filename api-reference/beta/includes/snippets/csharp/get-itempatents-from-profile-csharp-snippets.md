---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b87dfbbb3421c452240a36b89ebe3d187e84a4f
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46820136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var patents = await graphClient.Me.Profile.Patents
    .Request()
    .GetAsync();

```