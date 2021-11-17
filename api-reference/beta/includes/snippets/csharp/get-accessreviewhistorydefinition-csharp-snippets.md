---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 68499c4636cb5a5f2efeb89ed9a14a4a2c3a020c60cb2572ca65011ef407a36d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902699"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewHistoryDefinition = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions["{accessReviewHistoryDefinition-id}"]
    .Request()
    .GetAsync();

```