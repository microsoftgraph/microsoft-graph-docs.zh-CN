---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4875adfc02ac023aa6107c3228e4f2032dfb2cf9
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{id}"].Members.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```