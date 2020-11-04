---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52f42687603248e9444b8534c3de9a7ce1d0e7e5
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903651"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Groups["{id}"].Members
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Pr")
    .Select("displayName,id")
    .OrderBy("displayName ")
    .GetAsync();

```