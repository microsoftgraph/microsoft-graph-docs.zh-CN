---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ea5cc08e405a8b2e1d8e9be706a06437ac1454e3e06236218798ac3c0061a6e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = await graphClient.Policies.AccessReviewPolicy
    .Request()
    .GetAsync();

```