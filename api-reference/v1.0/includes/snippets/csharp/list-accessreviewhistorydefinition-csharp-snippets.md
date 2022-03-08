---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74433e3d15a180b1aba2324a1f23b851603690e6
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337665"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var historyDefinitions = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions
    .Request()
    .GetAsync();

```