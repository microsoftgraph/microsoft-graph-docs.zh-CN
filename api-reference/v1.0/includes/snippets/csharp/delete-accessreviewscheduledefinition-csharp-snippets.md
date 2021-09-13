---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 304957dd33a1d746dde31e586f4c20d729a632d9bbccdeeb03a304539b8960d4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"]
    .Request()
    .DeleteAsync();

```