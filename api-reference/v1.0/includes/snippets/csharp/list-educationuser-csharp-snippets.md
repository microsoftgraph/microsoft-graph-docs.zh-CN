---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b92af20fa2cc2478a06a940db6f1f9267a0c1803c566c6e5c0fb5a2188ce1352
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var users = await graphClient.Education.Users
    .Request()
    .GetAsync();

```