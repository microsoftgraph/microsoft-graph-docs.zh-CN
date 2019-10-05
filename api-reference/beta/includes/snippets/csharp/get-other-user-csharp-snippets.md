---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6bbaabcd8c30664bf9d4f3468a996a17ddf9b27b
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402438"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{id}"]
    .Request()
    .GetAsync();

```