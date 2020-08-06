---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46fc470f13844e0d452a9002ad432a2bdae3eda9
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46569993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Oauth2permissiongrants
    .Delta()
    .Request()
    .GetAsync();

```