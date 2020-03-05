---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bfccbb519a33ff8ffadf9105311770bea9f8869
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476534"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var stream = await graphClient.Me.Messages["4aade2547798441eab5188a7a2436bc1"].Content
    .Request()
    .GetAsync();

```