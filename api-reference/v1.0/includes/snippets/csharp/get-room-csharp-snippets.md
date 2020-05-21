---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26a7a56142188af60d369178ed864cb7ba4a3bad
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = await graphClient.Places["3162F1E1-C4C0-604B-51D8-91DA78989EB1"]
    .Request()
    .GetAsync();

```