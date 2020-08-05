---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce734851210eb4f0f649950fe8fd284456f72ed6
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46570048"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Organization["{organizationId}"].Settings.ProfileCardProperties["fax"]
    .Request()
    .DeleteAsync();

```