---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7f247fbe360e71e1ff6061050aa831158f673f50c006a80fe83fa6a204481df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104142"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstance = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .Request()
    .GetAsync();

```