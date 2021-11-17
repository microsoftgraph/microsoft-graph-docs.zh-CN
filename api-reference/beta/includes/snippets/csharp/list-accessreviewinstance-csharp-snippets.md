---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7efd14bfffbd139d2389adca1139ca4e6c4f0656554cf81ccf4a7f519b348feb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902676"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```