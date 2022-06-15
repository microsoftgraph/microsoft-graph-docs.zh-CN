---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52a4c17d507ad61f7d57a56708a456d96014e633
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093168"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassAuthenticationMethod = await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods["{temporaryAccessPassAuthenticationMethod-id}"]
    .Request()
    .GetAsync();

```