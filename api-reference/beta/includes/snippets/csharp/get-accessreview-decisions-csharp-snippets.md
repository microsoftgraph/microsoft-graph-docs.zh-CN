---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b1af56d995cb3a3aacd93b1f405d87961802557
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Decisions
    .Request()
    .GetAsync();

```