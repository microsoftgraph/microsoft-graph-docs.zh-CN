---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5efe02a18b6441db1738836fcca5833a19c25219
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176471"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissions = await graphClient.Sites["{sitesId}"].Permissions
    .Request()
    .GetAsync();

```