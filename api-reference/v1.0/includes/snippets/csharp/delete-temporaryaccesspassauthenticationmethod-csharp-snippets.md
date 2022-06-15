---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97bae033cce378db22d303169a588e063fff5018
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods["{temporaryAccessPassAuthenticationMethod-id}"]
    .Request()
    .DeleteAsync();

```