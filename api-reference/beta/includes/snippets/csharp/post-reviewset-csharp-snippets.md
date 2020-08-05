---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0b1c193535cb1b50687bcf1fb4d6d47578a11a69
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566244"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewSet = new ReviewSet
{
    DisplayName = "My Reviewset 3"
};

await graphClient.Compliance.Ediscovery.Cases["6f65a8e4-c6a0-4cff-8a81-c9ab5df7290d"].ReviewSets
    .Request()
    .AddAsync(reviewSet);

```