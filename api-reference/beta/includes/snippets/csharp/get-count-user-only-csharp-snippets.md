---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4875adfc02ac023aa6107c3228e4f2032dfb2cf9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{id}"].Members.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```