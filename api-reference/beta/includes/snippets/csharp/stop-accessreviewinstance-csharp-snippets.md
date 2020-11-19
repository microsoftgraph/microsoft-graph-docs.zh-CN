---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: a7d1c0b3a2fbff17f6271f79ee623ad07da547ac
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221990"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Instances["61a617dd-238f-4037-8fa5-d800e515f5bc"]
    .Stop()
    .Request()
    .PostAsync();

```