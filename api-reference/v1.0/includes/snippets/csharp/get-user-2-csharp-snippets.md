---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2bd84992456d4d605e7bf6b88e38fe3998d993f9
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .Select("displayName,givenName,postalCode")
    .GetAsync();

```