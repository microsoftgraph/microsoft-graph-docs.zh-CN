---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1165371ee3494106632f1ba97a22ba248c6163d
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225473"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactedReviewers = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].ContactedReviewers
    .Request()
    .GetAsync();

```