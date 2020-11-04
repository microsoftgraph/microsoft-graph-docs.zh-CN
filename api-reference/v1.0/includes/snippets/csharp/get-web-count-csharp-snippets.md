---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8acc4487316b7f38d40fe457fde943cde19c5c5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905584"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var applications = await graphClient.Applications
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Web")
    .GetAsync();

```