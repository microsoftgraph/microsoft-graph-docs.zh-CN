---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 642fd48ecf4ae647bd353d9433d39fe1cd73ca71
ms.sourcegitcommit: f50b1feff72182d1e19bfa346304beaf29558b68
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2019
ms.locfileid: "36461057"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Education.Me.Rubrics["{id}"]
    .Request()
    .DeleteAsync();

```