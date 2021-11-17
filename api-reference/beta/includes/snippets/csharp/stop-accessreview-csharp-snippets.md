---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03c153c0dfe08eccec1ed19f58b086f57d12d32532f21a91b3a8798797bead90
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158608"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .Stop()
    .Request()
    .PostAsync();

```