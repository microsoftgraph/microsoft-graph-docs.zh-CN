---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3619b06dd1433cfc939048ff7d35b5ebdbee6d79
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50433503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Account["{id}"]
    .Request()
    .DeleteAsync();

```