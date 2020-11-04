---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afbc0d8b69a2f7c20feac7538130db4512f5fa05
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{id}"].TransitiveMembers.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```