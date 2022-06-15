---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c61e5ec2cb6d99bec716dbe3ae77897dd4747956
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098664"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var temporaryAccessPassMethods = await graphClient.Users["{user-id}"].Authentication.TemporaryAccessPassMethods
    .Request()
    .GetAsync();

```