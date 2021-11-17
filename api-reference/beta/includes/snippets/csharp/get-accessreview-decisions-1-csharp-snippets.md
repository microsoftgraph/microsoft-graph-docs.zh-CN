---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3ba2e18dd7c3ea2afe1fae5c9f0c04f91c698fcedfdb4e361a9f53ced16b2cf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.AccessReviews["{accessReview-id}"].Decisions
    .Request()
    .GetAsync();

```