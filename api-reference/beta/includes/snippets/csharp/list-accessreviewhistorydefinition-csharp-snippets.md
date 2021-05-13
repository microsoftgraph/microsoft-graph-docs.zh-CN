---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74433e3d15a180b1aba2324a1f23b851603690e6
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var historyDefinitions = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions
    .Request()
    .GetAsync();

```