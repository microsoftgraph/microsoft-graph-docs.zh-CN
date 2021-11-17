---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4052f6705a121787cad0d64a5079bfef29e446aecd8c93b73dd1f3b7fdd15e7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902713"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```