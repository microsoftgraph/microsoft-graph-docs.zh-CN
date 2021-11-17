---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 304620552c7577811108eb82ee058d159e07c20c59c79c7621d7acdfae603ad8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = await graphClient.IdentityGovernance.AccessReviews.Policy
    .Request()
    .GetAsync();

```